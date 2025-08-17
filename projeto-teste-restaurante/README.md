# Projeto de Estudo: Planejamento de Testes para Sistema de Restaurante

Este repositório contém um projeto de estudo prático sobre Qualidade de Software (QA), baseado em um exercício de planejamento de testes para um sistema web de um restaurante. O conteúdo foi convertido do documento `Atividade_Pratica_Aula_3_Marcio_Lenes.pdf` para um formato adequado para um repositório Git.

## Contexto

Um restaurante está desenvolvendo um sistema web para gerenciamento de pedidos. O objetivo é permitir que os usuários realizem todo o fluxo de pedido de forma online, desde a escolha dos pratos até o acompanhamento da entrega.

### Funcionalidades do Sistema

As funcionalidades definidas para o sistema são:
- Visualizar o cardápio.
- Adicionar itens ao carrinho.
- Finalizar o pedido com forma de pagamento (PIX ou Cartão).
- Cancelar pedidos.
- Acompanhar o status do pedido (Recebido, Em preparo, Saiu para entrega, Entregue).

### Análise de Criticidade das Funcionalidades

Com base no impacto para o negócio e para o usuário, as funcionalidades foram priorizadas da seguinte forma:

- **CRÍTICA:** Finalizar Pedido com Pagamento. Uma falha aqui impede o faturamento e afeta diretamente a confiança do cliente.
- **ALTA:** Adicionar Itens ao Carrinho. Impede que o usuário monte seu pedido, bloqueando todo o fluxo.
- **ALTA:** Visualizar o Cardápio. É o ponto de entrada do sistema; se falhar, o usuário abandona a plataforma.
- **MÉDIA:** Acompanhar Status do Pedido. Importante para a experiência do cliente e para reduzir a ansiedade.
- **MÉDIA:** Cancelar Pedidos. Funcionalidade importante, mas com impacto menor que as demais.

## Estrutura do Repositório

- **`README.md`**: Este arquivo, com a introdução e o resumo do projeto.
- **`PLANO_DE_TESTES.md`**: Documento formal que descreve o escopo, objetivos, critérios, riscos e recursos para o ciclo de testes, baseado no Exercício 04.
- **`ESTRATEGIA_DE_TESTES.md`**: Descreve a abordagem geral, incluindo os níveis e tipos de teste a serem aplicados, conforme o Exercício 02.
- **`/cenarios-de-teste`**: Pasta contendo exemplos de casos de teste em Markdown, detalhando os passos para validar funcionalidades específicas.
  - `CT_001_Fluxo_Pedido_Completo.md`: Exemplo de cenário "caminho feliz".
  - `CT_002_Seguranca_Pagamento.md`: Detalhamento dos testes de segurança focados no checkout, baseado no Exercício 03.
  - `CT_003_Compatibilidade_Navegadores.md`: Exemplo de testes para múltiplos navegadores.

