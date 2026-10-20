# RF01 — Login e autenticação

Casos de teste funcionais seguindo o modelo de **Descrição → Pré-condições → Passos → Critérios de aceitação → Resultado → Status → Evidências**.

---

## Caso de Teste CT01: Login com credenciais válidas

| ID | Descrição |
|---|---|
| **RF01-CT01** | Verificar se um usuário cadastrado consegue autenticar com credenciais válidas. |

| Pré-condições |
|---|
| Usuário ativo e cadastrado no sistema. |

| Passos |
|---|
| DADO que estamos na página de login do Esfiharia Manager |
| E informamos um e-mail/usuário válido |
| E informamos uma senha válida |
| QUANDO clicarmos no botão de entrar |
| ENTÃO o sistema deve autenticar e redirecionar para a tela inicial |

| Critérios de aceitação |
|---|
| O sistema deve autenticar o usuário e exibir apenas as funcionalidades correspondentes ao seu perfil. |

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

## Caso de Teste CT02: Login com senha incorreta

| ID | Descrição |
|---|---|
| **RF01-CT02** | Verificar o bloqueio do login quando a senha estiver incorreta. |

| Pré-condições |
|---|
| Usuário ativo cadastrado. |

| Passos |
|---|
| DADO que estamos na página de login |
| E informamos um usuário válido |
| E informamos uma senha incorreta |
| QUANDO tentarmos entrar |
| ENTÃO o sistema deve negar a autenticação |

| Critérios de aceitação |
|---|
| O sistema deve permanecer na tela de login e informar que as credenciais são inválidas. |

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

## Caso de Teste CT03: Login com campos em branco

| ID | Descrição |
|---|---|
| **RF01-CT03** | Validar campos obrigatórios no login. |

| Pré-condições |
|---|
| Tela de login aberta. |

| Passos |
|---|
| DADO que estamos na tela de login |
| E não preenchemos usuário/e-mail e senha |
| QUANDO clicarmos em entrar |
| ENTÃO o sistema deve impedir o envio |

| Critérios de aceitação |
|---|
| Os campos obrigatórios devem ser validados e o usuário não deve ser autenticado. |

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

## Caso de Teste CT04: Login de usuário inativo

| ID | Descrição |
|---|---|
| **RF01-CT04** | Garantir que uma conta inativa não possa acessar o sistema. |

| Pré-condições |
|---|
| Usuário existente marcado como inativo. |

| Passos |
|---|
| DADO um usuário inativo |
| E informamos suas credenciais corretas |
| QUANDO tentarmos entrar |
| ENTÃO o acesso deve ser recusado |

| Critérios de aceitação |
|---|
| Usuário inativo não deve receber sessão válida. |

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
