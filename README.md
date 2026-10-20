# QA — Esfiharia Manager

Repositório destinado à **análise de qualidade (QA)** do sistema **Esfiharia Manager**, contemplando análise de requisitos, planejamento dos testes, cenários/casos de teste, registro de bugs e relatório de execução.

## Estrutura do repositório

```text
qa-esfiharia-manager/
├── README.md
├── 1-Analise-de-requisitos.md
├── 2-Plano-de-testes.md
├── 3-Relatorio-de-Bugs.md
├── 4-Relatorio-dos-testes.md
└── cenarios-de-testes/
    ├── CT_RF01_Login.md
    ├── CT_RF02_Recuperacao_de_Senha.md
    ├── CT_RF03_Perfis_e_Permissoes.md
    ├── CT_RF04_Usuarios.md
    ├── CT_RF05_Clientes.md
    ├── CT_RF06_Insumos_e_Estoque.md
    ├── CT_RF07_Produtos_e_Receitas.md
    ├── CT_RF08_Cardapio.md
    ├── CT_RF09_Pedidos.md
    ├── CT_RF10_Cozinha.md
    ├── CT_RF11_Cancelamentos_e_Estornos.md
    ├── CT_RF12_Caixa.md
    ├── CT_RF13_Entregas_e_Motoboy.md
    ├── CT_RF14_Relatorios.md
    ├── CT_RF15_Impressao.md
    ├── CT_RF16_Acompanhamento_do_Pedido.md
    ├── CT_RF17_Dashboard.md
    └── CT_RF18_Sessao_e_Logout.md
```

## Padrão utilizado

Os casos de teste seguem o formato apresentado no modelo fornecido:

- **ID**
- **Descrição**
- **Pré-condições**
- **Passos**, utilizando **DADO / E / QUANDO / ENTÃO**
- **Critérios de aceitação**
- **Resultado obtido**
- **Status**
- **Evidência(s)**

## Convenção dos IDs

- `CT_RF01` — Autenticação/Login
- `CT_RF02` — Recuperação de senha
- `CT_RF03` — Perfis e permissões
- `CT_RF04` — Usuários
- `CT_RF05` — Clientes
- `CT_RF06` — Insumos e estoque
- `CT_RF07` — Produtos e receitas
- `CT_RF08` — Cardápio
- `CT_RF09` — Pedidos
- `CT_RF10` — Cozinha
- `CT_RF11` — Cancelamentos e estornos
- `CT_RF12` — Caixa
- `CT_RF13` — Entregas/Motoboy
- `CT_RF14` — Relatórios
- `CT_RF15` — Impressão
- `CT_RF16` — Acompanhamento de pedido
- `CT_RF17` — Dashboard
- `CT_RF18` — Sessão e logout

Os casos internos usam a sequência `CT01`, `CT02`, `CT03` etc.

## Como utilizar

1. Executar cada caso no ambiente de testes.
2. Preencher **Resultado obtido**.
3. Alterar o **Status** para `Aprovado`, `Reprovado` ou `Bloqueado`.
4. Adicionar prints/vídeos na seção **Evidência(s)**.
5. Para falhas, registrar o defeito em `3-Relatorio-de-Bugs.md`.
6. Atualizar o consolidado em `4-Relatorio-dos-testes.md`.

## Status sugeridos

| Status | Significado |
|---|---|
| Não executado | Caso ainda não foi testado |
| Aprovado | Resultado obtido corresponde ao esperado |
| Reprovado | Resultado obtido diverge do esperado |
| Bloqueado | Não foi possível concluir o teste por dependência ou erro impeditivo |

## Sistema avaliado

O Esfiharia Manager centraliza autenticação, usuários, clientes, insumos, produtos/receitas, cardápio, pedidos, cozinha, caixa, entregas, relatórios e recursos auxiliares de operação.
