# RF02 — Recuperação de senha

Casos de teste funcionais seguindo o modelo de **Descrição → Pré-condições → Passos → Critérios de aceitação → Resultado → Status → Evidências**.

---

## Caso de Teste CT01: Solicitar recuperação de senha

| ID | Descrição |
|---|---|
| **RF02-CT01** | Validar o envio da solicitação de recuperação para usuário existente. |

| Pré-condições |
|---|
| Usuário com e-mail válido cadastrado. |

| Passos |
|---|
| DADO que estamos na opção de recuperar senha |
| E informamos um e-mail cadastrado |
| QUANDO confirmarmos a solicitação |
| ENTÃO o sistema deve gerar o procedimento de recuperação |

| Critérios de aceitação |
|---|
| O sistema deve confirmar a solicitação sem expor dados sensíveis. |

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

## Caso de Teste CT02: Redefinir senha por link válido

| ID | Descrição |
|---|---|
| **RF02-CT02** | Validar a criação de uma nova senha por link ainda válido. |

| Pré-condições |
|---|
| Link de recuperação válido e não expirado. |

| Passos |
|---|
| DADO que possuímos um link válido |
| E acessamos a página de redefinição |
| E informamos uma nova senha válida |
| QUANDO confirmarmos |
| ENTÃO a nova senha deve ser gravada |

| Critérios de aceitação |
|---|
| O login deve funcionar com a nova senha e deixar de funcionar com a anterior. |

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

## Caso de Teste CT03: Link de recuperação expirado

| ID | Descrição |
|---|---|
| **RF02-CT03** | Validar que links expirados não permitam redefinição. |

| Pré-condições |
|---|
| Link de recuperação com prazo expirado. |

| Passos |
|---|
| DADO que o link já expirou |
| QUANDO tentarmos acessá-lo ou salvar nova senha |
| ENTÃO o sistema deve bloquear a redefinição |

| Critérios de aceitação |
|---|
| O sistema deve informar expiração/invalidez e exigir nova solicitação. |

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
