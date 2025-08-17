# Plano de Testes - Sistema de Pedidos Web do Restaurante

## 1. Objetivo do Documento
[cite_start]O objetivo deste plano é descrever o escopo, a abordagem, os recursos e o cronograma das atividades de teste para o sistema de pedidos web do restaurante[cite: 96]. [cite_start]A meta principal é garantir que o sistema atenda a todos os requisitos funcionais e não funcionais, proporcionando uma experiência de alta qualidade para o usuário final[cite: 97].

## 2. Escopo dos Testes

### 2.1. Funcionalidades A SEREM Testadas (Em Escopo)
- [cite_start]Visualização completa do cardápio[cite: 101].
- [cite_start]Adição, edição e remoção de itens no carrinho de compras[cite: 102].
- [cite_start]Fluxo de finalização do pedido, incluindo o processo de pagamento com PIX e Cartão de Crédito[cite: 103].
- [cite_start]Funcionalidade de cancelamento de pedidos[cite: 103].
- [cite_start]Acompanhamento e atualização de status do pedido (Recebido, Em preparo, Saiu para entrega, Entregue)[cite: 104].

### 2.2. Funcionalidades a NÃO SEREM Testadas (Fora de Escopo)
- Painel administrativo do restaurante (gerenciamento de cardápio, visualização de pedidos, etc.).
- Testes de carga e estresse aprofundados (apenas testes de performance básicos serão executados).
- Módulo de cadastro e autenticação de usuários (considerado como pré-condição).

## 3. Critérios de Entrada e Saída

### 3.1. Critérios de Entrada (Para iniciar os testes)
- [cite_start]O ambiente de testes (homologação) deve estar configurado e estável[cite: 107].
- [cite_start]A build da versão a ser testada deve estar instalada no ambiente[cite: 108].
- [cite_start]Este plano de testes deve estar revisado e aprovado[cite: 109].
- [cite_start]A massa de dados para os testes (usuários, produtos, cartões de teste) deve estar preparada[cite: 110].

### 3.2. Critérios de Saída (Para finalizar os testes)
- [cite_start]100% dos casos de teste com prioridade Crítica e Alta devem ser executados[cite: 112].
- [cite_start]Nenhum defeito com severidade Crítica (impeditivo/blocker) pode estar em aberto[cite: 112].
- [cite_start]Todos os defeitos com severidade Alta devem estar corrigidos e verificados[cite: 113].
- [cite_start]O relatório final de testes deve ser gerado e compartilhado com os stakeholders[cite: 113].

## 4. Riscos Conhecidos
- [cite_start]**Risco 1:** Falha na integração com o gateway de pagamento, impedindo transações[cite: 115].
- [cite_start]**Risco 2:** Cálculo incorreto do valor total do pedido (soma de itens + taxa de entrega)[cite: 116].
- [cite_start]**Risco 3:** O status do pedido não ser atualizado em tempo real para o cliente[cite: 116].
- [cite_start]**Risco 4:** Inconsistências de layout e funcionalidade em diferentes dispositivos e navegadores[cite: 116].

## 5. Ambiente, Ferramentas e Recursos

### 5.1. Ambientes Necessários
- [cite_start]**Navegadores:** Google Chrome (última versão), Mozilla Firefox (última versão), Safari (última versão)[cite: 118].
- [cite_start]**Dispositivos:** Desktop (Windows/macOS) e Mobile (emulação via DevTools para viewports de iPhone e Android populares)[cite: 119].

### 5.2. Ferramentas
- [cite_start]**Gestão de Testes e Defeitos:** Jira, Trello ou Planilha Google[cite: 120].
- [cite_start]**Automação (sugestão):** Cypress ou Selenium para automatizar os fluxos críticos[cite: 121].