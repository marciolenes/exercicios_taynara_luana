# Projeto de Estudo: Planejamento de Testes para Sistema de Restaurante

Este repositório contém um projeto de estudo prático sobre Qualidade de Software (QA), baseado em um exercício de planejamento de testes para um sistema web de um restaurante. O conteúdo foi convertido do documento `Atividade Pratica - Aula 3 - Marcio Lenes.pdf` para um formato adequado para um repositório Git.

## Contexto

[cite_start]Um restaurante está desenvolvendo um sistema web para gerenciamento de pedidos[cite: 7, 125]. O objetivo é permitir que os usuários realizem todo o fluxo de pedido de forma online, desde a escolha dos pratos até o acompanhamento da entrega.

### Funcionalidades do Sistema

As funcionalidades definidas para o sistema são:
- [cite_start]Visualizar o cardápio[cite: 8, 30, 54, 82, 101, 126].
- [cite_start]Adicionar itens ao carrinho[cite: 9, 31, 55, 83, 102, 127].
- [cite_start]Finalizar o pedido com forma de pagamento (PIX ou Cartão)[cite: 10, 32, 56, 84, 103, 128].
- [cite_start]Cancelar pedidos[cite: 10, 32, 57, 84, 103].
- [cite_start]Acompanhar o status do pedido (Recebido, Em preparo, Saiu para entrega, Entregue)[cite: 11, 33, 58, 85, 104, 129].

### Análise de Criticidade das Funcionalidades

Com base no impacto para o negócio e para o usuário, as funcionalidades foram priorizadas da seguinte forma:

- **CRÍTICA:** Finalizar Pedido com Pagamento. [cite_start]Uma falha aqui impede o faturamento e afeta diretamente a confiança do cliente[cite: 18, 19].
- **ALTA:** Adicionar Itens ao Carrinho. [cite_start]Impede que o usuário monte seu pedido, bloqueando todo o fluxo[cite: 20].
- **ALTA:** Visualizar o Cardápio. [cite_start]É o ponto de entrada do sistema; se falhar, o usuário abandona a plataforma[cite: 21, 22].
- **MÉDIA:** Acompanhar Status do Pedido. [cite_start]Importante para a experiência do cliente e para reduzir a ansiedade[cite: 23].
- **MÉDIA:** Cancelar Pedidos. [cite_start]Funcionalidade importante, mas com impacto menor que as demais[cite: 24].

## Estrutura do Repositório

- **`README.md`**: Este arquivo, com a introdução e o resumo do projeto.
- [cite_start]**`PLANO_DE_TESTES.md`**: Documento formal que descreve o escopo, objetivos, critérios, riscos e recursos para o ciclo de testes, baseado no Exercício 04[cite: 79].
- [cite_start]**`ESTRATEGIA_DE_TESTES.md`**: Descreve a abordagem geral, incluindo os níveis e tipos de teste a serem aplicados, conforme o Exercício 02[cite: 25].
- **`/cenarios-de-teste`**: Pasta contendo exemplos de casos de teste em Markdown, detalhando os passos para validar funcionalidades específicas.
  - `CT_001_Fluxo_Pedido_Completo.md`: Exemplo de cenário "caminho feliz".
  - [cite_start]`CT_002_Seguranca_Pagamento.md`: Detalhamento dos testes de segurança focados no checkout, baseado no Exercício 03[cite: 49].
  - `CT_003_Compatibilidade_Navegadores.md`: Exemplo de testes para múltiplos navegadores.