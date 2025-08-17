# Cenário de Teste: CT_003 - Compatibilidade em Navegadores e Dispositivos

**Funcionalidade:** Validação de Interface e Layout

**Prioridade:** ALTA

---

**Objetivo:** Garantir que o sistema seja funcional e visualmente consistente nos navegadores e dispositivos mais populares.

**Pré-condições:**
- O fluxo de pedido completo (CT_001) deve ser usado como base para a execução em cada ambiente.

---

### Ambientes de Teste:
- **Navegador 1:** Google Chrome (Última versão) em Desktop.
- **Navegador 2:** Mozilla Firefox (Última versão) em Desktop.
- **Navegador 3:** Safari (Última versão) em macOS.
- **Dispositivo 4:** Emulador do Chrome DevTools - Viewport "iPhone 12 Pro".
- **Dispositivo 5:** Emulador do Chrome DevTools - Viewport "Samsung Galaxy S20 Ultra".

---

### Passos de Verificação (executar em cada ambiente):

| Verificação | Critério de Aceite |
| :--- | :--- |
| **1. Visualização do Cardápio** | Os nomes, descrições, preços e imagens dos produtos são exibidos corretamente, sem quebras de layout. |
| **2. Adição ao Carrinho** | O botão "Adicionar" está visível e clicável. A confirmação visual da adição funciona. |
| **3. Página do Carrinho** | Todos os elementos (itens, preços, botão de finalizar) estão visíveis e alinhados corretamente. |
| **4. Página de Checkout** | Os campos de formulário estão alinhados, legíveis e totalmente funcionais. Não há sobreposição de elementos. |
| **5. Modais e Pop-ups** | Mensagens de confirmação ou erro são exibidas de forma centralizada e são responsivas. |

**Resultado Esperado:** O fluxo completo deve ser concluído com sucesso em todos os ambientes listados, sem apresentar defeitos visuais ou funcionais críticos.

