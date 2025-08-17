# Cenário de Teste: CT_002 - Segurança no Checkout

**Funcionalidade:** Finalização de Pedido (Segurança)
**Prioridade:** CRÍTICA

---

[cite_start]**Objetivo:** Garantir a confidencialidade, integridade e segurança dos dados do cliente durante o processo de pagamento, conforme a análise de vulnerabilidades[cite: 62].

---

### [cite_start]1. Validação de Campos de Entrada [cite: 64]
- **Cenário 1.1:** Tentar inserir scripts (XSS) nos campos de nome, endereço e dados do cartão.
  - **Resultado Esperado:** O sistema deve sanitizar as entradas e não executar o script.
- [cite_start]**Cenário 1.2:** Tentar inserir comandos SQL (SQL Injection) nos campos de entrada[cite: 65].
  - **Resultado Esperado:** O sistema deve tratar a entrada como texto e não executar a query no banco de dados.
- [cite_start]**Cenário 1.3:** Inserir formatos inválidos nos campos do cartão (ex: número com letras, data de validade no passado)[cite: 66].
  - **Resultado Esperado:** O sistema deve exibir mensagens de erro claras e não permitir o envio do formulário.

### 2. Transmissão e Armazenamento de Dados
- [cite_start]**Cenário 2.1:** Verificar se a página de checkout utiliza o protocolo HTTPS[cite: 68].
  - **Resultado Esperado:** O cadeado de segurança deve estar visível no navegador e o tráfego de dados deve ser criptografado.
- [cite_start]**Cenário 2.2:** Após uma transação bem-sucedida, verificar no banco de dados se o número completo do cartão e o CVV foram armazenados[cite: 71].
  - [cite_start]**Resultado Esperado:** O sistema **NÃO** deve armazenar esses dados sensíveis[cite: 71].

### [cite_start]3. Gerenciamento de Sessão [cite: 73]
- **Cenário 3.1:** Após finalizar um pedido, fazer logout e tentar acessar a URL da página de confirmação novamente.
  - **Resultado Esperado:** O sistema deve redirecionar para a página de login ou para a página inicial, impedindo o acesso.
- [cite_start]**Cenário 3.2:** Tentar manipular a URL com o ID de sessão de outro usuário para acessar seu checkout[cite: 75].
  - **Resultado Esperado:** O acesso deve ser negado.

### [cite_start]4. Integração com Gateway de Pagamento [cite: 76]
- [cite_start]**Cenário 4.1:** Realizar um pagamento com um cartão de teste que simule uma transação negada pelo banco[cite: 78].
  - [cite_start]**Resultado Esperado:** O sistema deve exibir uma mensagem amigável informando que o pagamento foi recusado e não expor detalhes técnicos do erro[cite: 78].