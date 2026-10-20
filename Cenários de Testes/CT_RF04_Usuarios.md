# RF04 — Cadastro e manutenção de usuários

Casos de teste funcionais seguindo o modelo de **Descrição → Pré-condições → Passos → Critérios de aceitação → Resultado → Status → Evidências**.

---

## Caso de Teste CT01: Cadastrar usuário válido

| ID | Descrição |
|---|---|
| **RF04-CT01** | Validar cadastro de novo usuário com dados obrigatórios. |

| Pré-condições |
|---|
| Administrador autenticado. |

| Passos |
|---|
| DADO que estamos na tela de usuários |
| E clicamos em novo usuário |
| E preenchemos os campos válidos |
| QUANDO salvarmos |
| ENTÃO o usuário deve ser cadastrado |

| Critérios de aceitação |
|---|
| O novo usuário deve aparecer na consulta com o perfil e status informados. |

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

## Caso de Teste CT02: Impedir cadastro inválido

| ID | Descrição |
|---|---|
| **RF04-CT02** | Validar campos obrigatórios e duplicidades. |

| Pré-condições |
|---|
| Administrador autenticado. |

| Passos |
|---|
| DADO que iniciamos um cadastro |
| E deixamos dados obrigatórios inválidos ou duplicados |
| QUANDO salvarmos |
| ENTÃO o sistema deve recusar o cadastro |

| Critérios de aceitação |
|---|
| Não deve ser criado registro inválido ou duplicado. |

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

## Caso de Teste CT03: Editar e inativar usuário

| ID | Descrição |
|---|---|
| **RF04-CT03** | Validar alteração de dados e status. |

| Pré-condições |
|---|
| Usuário existente. |

| Passos |
|---|
| DADO que localizamos um usuário existente |
| E alteramos seus dados ou status |
| QUANDO salvarmos |
| ENTÃO as alterações devem persistir |

| Critérios de aceitação |
|---|
| Usuário inativado deve permanecer consultável, mas sem acesso ao sistema. |

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
