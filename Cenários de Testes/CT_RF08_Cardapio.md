# RF08 — Cardápio

Casos de teste funcionais seguindo o modelo de **Descrição → Pré-condições → Passos → Critérios de aceitação → Resultado → Status → Evidências**.

---

## Caso de Teste CT01: Exibir produtos disponíveis

| ID | Descrição |
|---|---|
| **RF08-CT01** | Validar a exibição dos produtos ativos e disponíveis. |

| Pré-condições |
|---|
| Existem produtos ativos com estoque suficiente. |

| Passos |
|---|
| DADO que acessamos o cardápio |
| QUANDO os produtos forem carregados |
| ENTÃO os itens disponíveis devem ser exibidos |

| Critérios de aceitação |
|---|
| Nome, preço e demais informações necessárias devem estar coerentes. |

| Resultado obtido |
|---|
| A preencher após a execução. |

| Status |
|---|
| Não executado. |

| Evidência(s) |
|---|
| Print da execução: a inserir. |

---

## Caso de Teste CT02: Bloquear produto sem insumo

| ID | Descrição |
|---|---|
| **RF08-CT02** | Validar indisponibilidade por falta de insumo. |

| Pré-condições |
|---|
| Produto cuja receita depende de insumo sem saldo. |

| Passos |
|---|
| DADO que um produto não possui insumos suficientes |
| QUANDO acessarmos o cardápio |
| ENTÃO o produto deve ser sinalizado ou bloqueado |

| Critérios de aceitação |
|---|
| O usuário não deve concluir inclusão de produto indisponível. |

| Resultado obtido |
|---|
| A preencher após a execução. |

| Status |
|---|
| Não executado. |

| Evidência(s) |
|---|
| Print da execução: a inserir. |

---

## Caso de Teste CT03: Estoque acaba durante o pedido

| ID | Descrição |
|---|---|
| **RF08-CT03** | Validar rechecagem de disponibilidade antes de concluir. |

| Pré-condições |
|---|
| Produto inicialmente disponível e estoque alterado antes da confirmação. |

| Passos |
|---|
| DADO que adicionamos um produto ao pedido |
| E o estoque fica insuficiente antes da confirmação |
| QUANDO tentarmos concluir |
| ENTÃO o sistema deve revalidar a disponibilidade |

| Critérios de aceitação |
|---|
| O pedido não deve ser finalizado com item sem estoque suficiente. |

| Resultado obtido |
|---|
| A preencher após a execução. |

| Status |
|---|
| Não executado. |

| Evidência(s) |
|---|
| Print da execução: a inserir. |

---
