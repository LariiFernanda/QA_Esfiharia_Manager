# RF10 — Cozinha

Casos de teste funcionais seguindo o modelo de **Descrição → Pré-condições → Passos → Critérios de aceitação → Resultado → Status → Evidências**.

---

## Caso de Teste CT01: Receber novo pedido

| ID | Descrição |
|---|---|
| **RF10-CT01** | Validar entrada de novo pedido em Recebidos. |

| Pré-condições |
|---|
| Pedido recém-criado. |

| Passos |
|---|
| DADO que um pedido válido foi lançado |
| QUANDO acessarmos a cozinha |
| ENTÃO o pedido deve aparecer em Recebidos |

| Critérios de aceitação |
|---|
| Itens e informações de preparo devem estar disponíveis. |

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

## Caso de Teste CT02: Mover para Produção

| ID | Descrição |
|---|---|
| **RF10-CT02** | Validar início do preparo. |

| Pré-condições |
|---|
| Pedido em Recebidos. |

| Passos |
|---|
| DADO que existe um pedido em Recebidos |
| QUANDO alterarmos para Produção |
| ENTÃO o pedido deve migrar de etapa |

| Critérios de aceitação |
|---|
| O novo status deve refletir imediatamente. |

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

## Caso de Teste CT03: Mover para Pronto

| ID | Descrição |
|---|---|
| **RF10-CT03** | Validar conclusão do preparo e regra de estoque. |

| Pré-condições |
|---|
| Pedido em Produção. |

| Passos |
|---|
| DADO que existe pedido em Produção |
| QUANDO marcarmos como Pronto |
| ENTÃO o pedido deve mudar de status e aplicar a regra de baixa de insumos |

| Critérios de aceitação |
|---|
| O estoque e o status devem ficar consistentes. |

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

## Caso de Teste CT04: Liberar para Entrega/Retirada

| ID | Descrição |
|---|---|
| **RF10-CT04** | Validar saída da cozinha após pronto. |

| Pré-condições |
|---|
| Pedido em Pronto. |

| Passos |
|---|
| DADO que o pedido está Pronto |
| QUANDO for liberado conforme o tipo de atendimento |
| ENTÃO deve avançar para entrega/retirada |

| Critérios de aceitação |
|---|
| O pedido não deve permanecer indevidamente na fila de produção. |

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
