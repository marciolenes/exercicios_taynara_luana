# Cenário de Teste: CT_001 - Fluxo de Pedido Completo (Caminho Feliz)

**Funcionalidade:** Finalização de Pedido
**Prioridade:** CRÍTICA

---

**Objetivo:** Validar o fluxo completo de um pedido bem-sucedido, desde a seleção do item até a confirmação do pagamento com Cartão de Crédito.

**Pré-condições:**
- O usuário está na página inicial do restaurante.
- O cardápio está carregado com itens disponíveis.

---

| Passo | Ação | Resultado Esperado |
| :--- | :--- | :--- |
| 1 | Navegar pelo cardápio e clicar em "Adicionar" em um item. | O item é adicionado ao carrinho e um contador no ícone do carrinho é atualizado. |
| 2 | Clicar no ícone do carrinho. | O sistema redireciona para a página do carrinho, exibindo o item adicionado e o valor total. |
| 3 | Clicar em "Finalizar Pedido". | O sistema redireciona para a página de checkout/pagamento. |
| 4 | Preencher os campos de endereço de entrega. | Os campos aceitam os dados corretamente. |
| 5 | Selecionar "Cartão de Crédito" como forma de pagamento. | Os campos para dados do cartão (número, nome, validade, CVV) são exibidos. |
| 6 | Preencher os campos com dados de um cartão de teste válido. | O sistema aceita os dados sem erros. |
| 7 | Clicar em "Confirmar Pagamento". | O pagamento é processado e o sistema exibe uma mensagem de "Pedido realizado com sucesso!". |
| 8 | Navegar para a tela "Meus Pedidos". | O novo pedido é exibido com o status "Recebido". |