# Projeto Final - CT - Ordenação e Prioridade

# Projeto Final

Chegamos ao projeto final deste Coding Tank. Aqui você vai encontrar a descrição do problema a ser resolvido e as instruções de formatação - apenas quanto às sessões e conteúdo - do documento a ser entregue.

## Cenário fictício: Marketplace Priority Sorter (MPS)

O *VelozMart*, grande empresa de logística e varejo da América Latina, lançou uma feature que mostra em tempo real uma lista de **pedidos** aguardando expedição. O objetivo é exibir os pedidos na **ordem ótima** para minimizar atrasos e custos logísticos.

### Elementos do problema

* Cada pedido possui:

  + *priorityScore* (0–100) calculado por IA com base em distância, SLA, valor do item e reputação do vendedor.
  + *dispatchWindow* (minutos restantes até prazo expirar).
  + *sizeCategory* (P, M, G) que impacta espaço na doca de embalagem.

* O time de logística pediu um **protótipo conceitual** que responda:

  1. Como **ordenar** pedidos considerando múltiplos critérios?
  2. Como re‑**enfileirar** pedidos à medida que novos chegam ou prazos mudam?
  3. Quais métricas comprovam que a estratégia é melhor que uma ordenação simples por tempo?

> Existem diversas estratégias válidas: peso composto (priorityScore × 1/dispatchWindow), duas filas (urgentes vs. normais), heap multi‑chave, algoritmo de aproximação de scheduling, etc. A escolha é livre, desde que fundamentada.

### Requisitos mínimos da solução

1. **Descrição textual do algoritmo/estrutura** escolhida (pseudocódigo opcional).
2. **Diagrama** (heap, fluxo, ou gráfico de Gantt) explicando o processo de inclusão, remoção e re‑priorização.
3. **Justificativa** dos critérios de ordenação e efeitos sobre métricas logísticas (p.ex. atraso médio, throughput/hora).
4. **Mapa de trade‑offs** (simplicidade × desempenho × manutenibilidade).

Itens bônus (não obrigatórios): análise Big O, comparação entre duas abordagens, proposta de teste A/B ou simulação, discussão de acessibilidade na UI.

## Template de entrega (Canvas‑PDF)

Considere o template abaixo descrevendo as sessões que devem ter no documento a ser entregue como solução para o projeto.

| Seção | Guia de conteúdo |
| --- | --- |
| **Problema** | Situação real resumida em 3–4 linhas; dados de contexto. |
| **Algoritmo / Estrutura** | Nome, motivação e breve pseudocódigo. |
| **Diagrama** | Imagem autoexplicativa; use legenda e alto contraste. |
| **Trade‑offs** | 3 prós & 3 contras; justificativa de escolha. |
| **Próximos passos** | Ideias futuras (ex.: incorporar aprendizagem online). |
