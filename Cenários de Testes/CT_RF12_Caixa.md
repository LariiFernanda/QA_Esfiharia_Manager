# RF12 — Caixa

Casos de teste funcionais seguindo o modelo de **Descrição → Pré-condições → Passos → Critérios de aceitação → Resultado → Status → Evidências**.

---

## Caso de Teste CT01: Abrir caixa

| ID | Descrição |
|---|---|
| **RF12-CT01** | Validar abertura de nova sessão. |

| Pré-condições |
|---|
| Não existe caixa aberto. |

| Passos |
|---|
| DADO que acessamos o módulo Caixa |
| QUANDO abrirmos uma sessão com o valor inicial |
| ENTÃO uma nova sessão deve ser criada |

| Critérios de aceitação |
|---|
| Somente uma sessão pode permanecer aberta por vez. |

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

## Caso de Teste CT02: Registrar entrada/saída manual

| ID | Descrição |
|---|---|
| **RF12-CT02** | Validar movimentações manuais autorizadas. |

| Pré-condições |
|---|
| Caixa aberto. |

| Passos |
|---|
| DADO que há uma sessão aberta |
| E escolhemos entrada ou saída |
| E informamos valor e justificativa |
| QUANDO salvarmos |
| ENTÃO a movimentação deve ser registrada |

| Critérios de aceitação |
|---|
| O saldo e o histórico devem refletir a operação. |

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

## Caso de Teste CT03: Fechar caixa com conferência

| ID | Descrição |
|---|---|
| **RF12-CT03** | Validar fechamento, valor contado e divergência. |

| Pré-condições |
|---|
| Caixa aberto com movimentações. |

| Passos |
|---|
| DADO que existe caixa aberto |
| E iniciamos a conferência |
| E informamos valores contados |
| QUANDO confirmarmos o fechamento |
| ENTÃO a sessão deve ser encerrada |

| Critérios de aceitação |
|---|
| Divergências devem exigir/registrar justificativa quando aplicável. |

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

## Caso de Teste CT04: Impedir múltiplos caixas abertos

| ID | Descrição |
|---|---|
| **RF12-CT04** | Validar exclusividade da sessão aberta. |

| Pré-condições |
|---|
| Já existe caixa aberto. |

| Passos |
|---|
| DADO que existe uma sessão de caixa aberta |
| QUANDO tentarmos abrir outra |
| ENTÃO o sistema deve bloquear a operação |

| Critérios de aceitação |
|---|
| O sistema não deve criar duas sessões simultaneamente. |

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
