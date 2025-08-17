# Estratégia de Testes

Esta seção detalha a abordagem e as metodologias de teste que serão adotadas para garantir a qualidade do sistema web do restaurante.

## 1. Níveis de Teste

- **Teste de Integração:** O foco será garantir que os diferentes módulos do sistema se comunicam corretamente. Por exemplo:
  - O carrinho de compras se integra ao módulo de finalização de pedido.
  - O módulo de finalização de pedido se integra ao sistema de pagamento externo (gateway).

- **Teste de Sistema:** Validaremos o sistema web como um todo, executando fluxos de ponta a ponta (end-to-end) que simulam a jornada completa do usuário. Isso inclui desde a visualização do cardápio até o recebimento da confirmação do pedido.

## 2. Tipos de Teste

- **Testes Funcionais:** Serão o foco principal do esforço, garantindo que todas as funcionalidades listadas no escopo operem conforme os requisitos.

- **Testes de Usabilidade e UI (Interface do Usuário):** Avaliaremos se o sistema é intuitivo, fácil de usar e se a interface é consistente e agradável em diferentes dispositivos.

- **Testes de Compatibilidade:** Sendo um sistema web, é crucial validar seu funcionamento nos navegadores mais populares (Chrome, Firefox, Safari) e em diferentes resoluções de tela (Desktop, Tablet e Mobile).

- **Testes de Performance:** Mediremos os tempos de resposta de ações críticas, como o carregamento do cardápio e o processamento do pagamento, para garantir uma experiência de uso fluida.

- **Testes de Segurança:** Validaremos vulnerabilidades básicas, como garantir que um usuário não possa acessar ou interferir no pedido de outro, com foco especial na proteção dos dados de pagamento.
