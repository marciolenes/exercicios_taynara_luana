# Estratégia de Testes

Esta seção detalha a abordagem e as metodologias de teste que serão adotadas para garantir a qualidade do sistema web do restaurante.

## 1. Níveis de Teste

- [cite_start]**Teste de Integração:** O foco será garantir que os diferentes módulos do sistema se comunicam corretamente[cite: 39]. Por exemplo:
  - [cite_start]O carrinho de compras se integra ao módulo de finalização de pedido[cite: 40].
  - [cite_start]O módulo de finalização de pedido se integra ao sistema de pagamento externo (gateway)[cite: 40].

- [cite_start]**Teste de Sistema:** Validaremos o sistema web como um todo, executando fluxos de ponta a ponta (end-to-end) que simulam a jornada completa do usuário[cite: 41]. [cite_start]Isso inclui desde a visualização do cardápio até o recebimento da confirmação do pedido[cite: 41].

## 2. Tipos de Teste

- [cite_start]**Testes Funcionais:** Serão o foco principal do esforço, garantindo que todas as funcionalidades listadas no escopo operem conforme os requisitos[cite: 43, 44].

- [cite_start]**Testes de Usabilidade e UI (Interface do Usuário):** Avaliaremos se o sistema é intuitivo, fácil de usar e se a interface é consistente e agradável em diferentes dispositivos[cite: 45].

- [cite_start]**Testes de Compatibilidade:** Sendo um sistema web, é crucial validar seu funcionamento nos navegadores mais populares (Chrome, Firefox, Safari) e em diferentes resoluções de tela (Desktop, Tablet e Mobile)[cite: 46].

- [cite_start]**Testes de Performance:** Mediremos os tempos de resposta de ações críticas, como o carregamento do cardápio e o processamento do pagamento, para garantir uma experiência de uso fluida[cite: 47].

- [cite_start]**Testes de Segurança:** Validaremos vulnerabilidades básicas, como garantir que um usuário não possa acessar ou interferir no pedido de outro [cite: 48][cite_start], com foco especial na proteção dos dados de pagamento[cite: 62].