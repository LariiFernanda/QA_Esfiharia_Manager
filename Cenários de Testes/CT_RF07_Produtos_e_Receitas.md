# RF07 — Produtos e receitas

Casos de teste funcionais seguindo o modelo de **Descrição → Pré-condições → Passos → Critérios de aceitação → Resultado → Status → Evidências**.

---

## Caso de Teste CT01: Cadastrar produto com receita

| ID | Descrição |
|---|---|
| **RF07-CT01** | Validar produto final associado a insumos. |

| Pré-condições |
|---|
| Administrador autenticado e insumos cadastrados. |

| Passos |
|---|
| DADO que abrimos o cadastro de produtos |
| E informamos os dados do produto |
| E adicionamos insumos e quantidades da receita |
| QUANDO salvarmos |
| ENTÃO o produto deve ser cadastrado |

| Critérios de aceitação |
|---|
| O produto deve manter a composição informada. |

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

## Caso de Teste CT02: Editar produto/receita

| ID | Descrição |
|---|---|
| **RF07-CT02** | Validar alteração de dados e composição. |

| Pré-condições |
|---|
| Produto existente. |

| Passos |
|---|
| DADO que localizamos um produto |
| E alteramos preço, dados ou receita |
| QUANDO salvarmos |
| ENTÃO as mudanças devem persistir |

| Critérios de aceitação |
|---|
| A consulta posterior deve exibir os novos dados. |

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

## Caso de Teste CT03: Inativar produto

| ID | Descrição |
|---|---|
| **RF07-CT03** | Validar que produto inativo não seja oferecido normalmente no cardápio. |

| Pré-condições |
|---|
| Produto ativo existente. |

| Passos |
|---|
| DADO que selecionamos um produto ativo |
| QUANDO o inativarmos |
| ENTÃO o status deve ser salvo |

| Critérios de aceitação |
|---|
| Produto inativo não deve ser disponibilizado para novos pedidos. |

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
