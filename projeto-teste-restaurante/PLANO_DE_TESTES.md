# Plano de Testes - Sistema de Pedidos Web do Restaurante

## 1. Objetivo do Documento
O objetivo deste plano é descrever o escopo, a abordagem, os recursos e o cronograma das atividades de teste para o sistema de pedidos web do restaurante. A meta principal é garantir que o sistema atenda a todos os requisitos funcionais e não funcionais, proporcionando uma experiência de alta qualidade para o usuário final.

## 2. Escopo dos Testes

### 2.1. Funcionalidades A SEREM Testadas (Em Escopo)
- Visualização completa do cardápio.
- Adição, edição e remoção de itens no carrinho de compras.
- Fluxo de finalização do pedido, incluindo o processo de pagamento com PIX e Cartão de Crédito.
- Funcionalidade de cancelamento de pedidos.
- Acompanhamento e atualização de status do pedido (Recebido, Em preparo, Saiu para entrega, Entregue).

### 2.2. Funcionalidades a NÃO SEREM Testadas (Fora de Escopo)
- Painel administrativo do restaurante (gerenciamento de cardápio, visualização de pedidos, etc.).
- Testes de carga e estresse aprofundados (apenas testes de performance básicos serão executados).
- Módulo de cadastro e autenticação de usuários (considerado como pré-condição).

## 3. Critérios de Entrada e Saída

### 3.1. Critérios de Entrada (Para iniciar os testes)
- O ambiente de testes (homologação) deve estar configurado e estável.
- A build da versão a ser testada deve estar instalada no ambiente.
- Este plano de testes deve estar revisado e aprovado.
- A massa de dados para os testes (usuários, produtos, cartões de teste) deve estar preparada.

### 3.2. Critérios de Saída (Para finalizar os testes)
- 100% dos casos de teste com prioridade Crítica e Alta devem ser executados.
- Nenhum defeito com severidade Crítica (impeditivo/blocker) pode estar em aberto.
- Todos os defeitos com severidade Alta devem estar corrigidos e verificados.
- O relatório final de testes deve ser gerado e compartilhado com os stakeholders.

## 4. Riscos Conhecidos
- **Risco 1:** Falha na integração com o gateway de pagamento, impedindo transações.
- **Risco 2:** Cálculo incorreto do valor total do pedido (soma de itens + taxa de entrega).
- **Risco 3:** O status do pedido não ser atualizado em tempo real para o cliente.
- **Risco 4:** Inconsistências de layout e funcionalidade em diferentes dispositivos e navegadores.

## 5. Ambiente, Ferramentas e Recursos

### 5.1. Ambientes Necessários
- **Navegadores:** Google Chrome (última versão), Mozilla Firefox (última versão), Safari (última versão).
- **Dispositivos:** Desktop (Windows/macOS) e Mobile (emulação via DevTools para viewports de iPhone e Android populares).

### 5.2. Ferramentas
- **Gestão de Testes e Defeitos:** Jira, Trello ou Planilha Google.
- **Automação (sugestão):** Cypress ou Selenium para automatizar os fluxos críticos.
