# RF03 — Perfis e permissões

Casos de teste funcionais seguindo o modelo de **Descrição → Pré-condições → Passos → Critérios de aceitação → Resultado → Status → Evidências**.

---

## Caso de Teste CT01: Acesso do Administrador

| ID | Descrição |
|---|---|
| **RF03-CT01** | Validar que o Administrador visualize os módulos administrativos. |

| Pré-condições |
|---|
| Usuário Administrador ativo. |

| Passos |
|---|
| DADO que efetuamos login como Administrador |
| QUANDO acessarmos o menu principal |
| ENTÃO os módulos administrativos permitidos devem estar disponíveis |

| Critérios de aceitação |
|---|
| O Administrador deve acessar cadastros, operações e relatórios previstos. |

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

## Caso de Teste CT02: Restrição do perfil Cozinha

| ID | Descrição |
|---|---|
| **RF03-CT02** | Validar que o perfil Cozinha não tenha acesso a funções financeiras/administrativas. |

| Pré-condições |
|---|
| Usuário Cozinha ativo. |

| Passos |
|---|
| DADO que efetuamos login como Cozinha |
| QUANDO navegarmos pelo sistema |
| ENTÃO somente funções relacionadas ao preparo devem estar disponíveis |

| Critérios de aceitação |
|---|
| Dados financeiros e cadastros administrativos não devem ser editáveis pelo perfil Cozinha. |

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

## Caso de Teste CT03: Restrição do perfil Motoboy

| ID | Descrição |
|---|---|
| **RF03-CT03** | Validar que o motoboy veja apenas suas funções de entrega. |

| Pré-condições |
|---|
| Usuário Motoboy ativo. |

| Passos |
|---|
| DADO que efetuamos login como Motoboy |
| QUANDO acessarmos o sistema |
| ENTÃO devem ser exibidas funções de entregas e relatório próprio |

| Critérios de aceitação |
|---|
| O motoboy não deve receber acesso indevido a cadastros ou configurações administrativas. |

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
