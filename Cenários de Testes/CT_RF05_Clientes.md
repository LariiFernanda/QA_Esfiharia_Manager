# RF05 — Clientes

Casos de teste funcionais seguindo o modelo de **Descrição → Pré-condições → Passos → Critérios de aceitação → Resultado → Status → Evidências**.

---

## Caso de Teste CT01: Cadastrar cliente

| ID | Descrição |
|---|---|
| **RF05-CT01** | Validar cadastro de cliente com dados válidos. |

| Pré-condições |
|---|
| Usuário autorizado autenticado. |

| Passos |
|---|
| DADO que abrimos o cadastro de clientes |
| E informamos os dados válidos |
| QUANDO salvarmos |
| ENTÃO o cliente deve ser cadastrado |

| Critérios de aceitação |
|---|
| O cliente deve estar disponível para pesquisa e uso em pedidos. |

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

## Caso de Teste CT02: Pesquisar cliente

| ID | Descrição |
|---|---|
| **RF05-CT02** | Validar pesquisa por dados suportados. |

| Pré-condições |
|---|
| Existem clientes cadastrados. |

| Passos |
|---|
| DADO que estamos na tela de clientes |
| E informamos nome, telefone, endereço ou e-mail |
| QUANDO clicarmos em pesquisar |
| ENTÃO os resultados compatíveis devem ser exibidos |

| Critérios de aceitação |
|---|
| A lista deve exibir apenas resultados coerentes com o termo e respeitar a paginação quando necessária. |

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

## Caso de Teste CT03: Bloquear cliente

| ID | Descrição |
|---|---|
| **RF05-CT03** | Validar bloqueio/desbloqueio de cliente. |

| Pré-condições |
|---|
| Cliente cadastrado. |

| Passos |
|---|
| DADO que selecionamos um cliente ativo |
| QUANDO alterarmos seu status para bloqueado |
| ENTÃO o bloqueio deve ser salvo |

| Critérios de aceitação |
|---|
| O status deve ficar visível e as regras de uso do cliente em novos pedidos devem ser respeitadas. |

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
