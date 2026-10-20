# RF11 — Cancelamentos e estornos

Casos de teste funcionais seguindo o modelo de **Descrição → Pré-condições → Passos → Critérios de aceitação → Resultado → Status → Evidências**.

---

## Caso de Teste CT01: Cancelar pedido recebido

| ID | Descrição |
|---|---|
| **RF11-CT01** | Validar cancelamento antes do preparo. |

| Pré-condições |
|---|
| Pedido em Recebidos. |

| Passos |
|---|
| DADO que existe pedido em Recebidos |
| QUANDO solicitarmos o cancelamento e informarmos o motivo |
| ENTÃO o pedido deve ir para Cancelados |

| Critérios de aceitação |
|---|
| O pedido não deve continuar no fluxo e os ajustes financeiros/estoque devem seguir a regra da etapa. |

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

## Caso de Teste CT02: Cancelar pedido pronto com destino

| ID | Descrição |
|---|---|
| **RF11-CT02** | Validar escolha entre reaproveitamento e descarte quando aplicável. |

| Pré-condições |
|---|
| Pedido em Pronto. |

| Passos |
|---|
| DADO que existe pedido em Pronto |
| QUANDO cancelarmos |
| E selecionarmos reaproveitamento ou descarte |
| ENTÃO o registro deve armazenar motivo, etapa e destino |

| Critérios de aceitação |
|---|
| O histórico de cancelamento deve ficar consultável. |

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

## Caso de Teste CT03: Registrar estorno com forma de pagamento

| ID | Descrição |
|---|---|
| **RF11-CT03** | Validar rastreabilidade financeira do estorno. |

| Pré-condições |
|---|
| Pedido elegível para estorno. |

| Passos |
|---|
| DADO que um pedido pago é cancelado |
| QUANDO registrarmos o estorno |
| ENTÃO a forma de pagamento do estorno deve ser registrada |

| Critérios de aceitação |
|---|
| Relatórios e caixa devem refletir o estorno corretamente, sem duplicidade. |

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
