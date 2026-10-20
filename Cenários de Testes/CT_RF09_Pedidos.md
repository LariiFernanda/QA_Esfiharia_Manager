# RF09 — Pedidos

Casos de teste funcionais seguindo o modelo de **Descrição → Pré-condições → Passos → Critérios de aceitação → Resultado → Status → Evidências**.

---

## Caso de Teste CT01: Criar pedido válido

| ID | Descrição |
|---|---|
| **RF09-CT01** | Validar lançamento completo de pedido. |

| Pré-condições |
|---|
| Usuário autorizado; cliente e produtos disponíveis. |

| Passos |
|---|
| DADO que estamos na tela de pedidos |
| E selecionamos um cliente |
| E adicionamos produtos |
| E definimos atendimento e pagamento |
| QUANDO confirmarmos o pedido |
| ENTÃO o pedido deve ser registrado |

| Critérios de aceitação |
|---|
| O pedido deve possuir total correto e entrar no fluxo operacional. |

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

## Caso de Teste CT02: Pedido sem forma de pagamento

| ID | Descrição |
|---|---|
| **RF09-CT02** | Validar obrigatoriedade da forma de pagamento. |

| Pré-condições |
|---|
| Pedido com cliente e itens. |

| Passos |
|---|
| DADO que preenchemos o pedido |
| E deixamos a forma de pagamento vazia |
| QUANDO tentarmos confirmar |
| ENTÃO o sistema deve impedir a conclusão |

| Critérios de aceitação |
|---|
| O sistema deve solicitar a forma de pagamento. |

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

## Caso de Teste CT03: Pedido sem itens

| ID | Descrição |
|---|---|
| **RF09-CT03** | Validar bloqueio de pedido vazio. |

| Pré-condições |
|---|
| Cliente selecionado. |

| Passos |
|---|
| DADO que selecionamos um cliente |
| E não adicionamos nenhum item |
| QUANDO tentarmos concluir |
| ENTÃO o sistema deve bloquear |

| Critérios de aceitação |
|---|
| Pedido vazio não deve ser gravado. |

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

## Caso de Teste CT04: Calcular entrega e total

| ID | Descrição |
|---|---|
| **RF09-CT04** | Validar subtotal, taxa de entrega e total. |

| Pré-condições |
|---|
| Pedido de entrega com itens. |

| Passos |
|---|
| DADO que adicionamos itens ao pedido |
| E definimos uma taxa de entrega |
| QUANDO o sistema calcular o total |
| ENTÃO subtotal + entrega devem resultar no total correto |

| Critérios de aceitação |
|---|
| Os valores exibidos e persistidos devem ser matematicamente consistentes. |

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
