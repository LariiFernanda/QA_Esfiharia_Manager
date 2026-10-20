# RF06 — Insumos e estoque

Casos de teste funcionais seguindo o modelo de **Descrição → Pré-condições → Passos → Critérios de aceitação → Resultado → Status → Evidências**.

---

## Caso de Teste CT01: Cadastrar insumo

| ID | Descrição |
|---|---|
| **RF06-CT01** | Validar cadastro de insumo com unidade, quantidade e mínimo. |

| Pré-condições |
|---|
| Administrador autenticado. |

| Passos |
|---|
| DADO que abrimos o cadastro de insumos |
| E preenchemos nome, unidade, saldo e mínimo |
| QUANDO salvarmos |
| ENTÃO o insumo deve ser criado |

| Critérios de aceitação |
|---|
| O insumo deve aparecer na listagem com os valores informados. |

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

## Caso de Teste CT02: Atualizar estoque

| ID | Descrição |
|---|---|
| **RF06-CT02** | Validar atualização de quantidade do insumo. |

| Pré-condições |
|---|
| Insumo existente. |

| Passos |
|---|
| DADO que existe um insumo cadastrado |
| QUANDO atualizarmos sua quantidade |
| ENTÃO o novo saldo deve ser persistido |

| Critérios de aceitação |
|---|
| A quantidade exibida deve refletir o valor salvo. |

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

## Caso de Teste CT03: Sinalizar estoque baixo/insuficiente

| ID | Descrição |
|---|---|
| **RF06-CT03** | Validar tratamento quando o saldo estiver abaixo do mínimo ou insuficiente. |

| Pré-condições |
|---|
| Insumo com saldo reduzido. |

| Passos |
|---|
| DADO que o estoque do insumo está baixo |
| QUANDO o sistema consultar sua disponibilidade |
| ENTÃO deve sinalizar a condição conforme a regra |

| Critérios de aceitação |
|---|
| Produtos dependentes de insumo insuficiente devem ser tratados como indisponíveis quando aplicável. |

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
