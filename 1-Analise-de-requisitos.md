# 1 — Análise de Requisitos

## 1. Objetivo

Esta análise tem como objetivo identificar as principais funcionalidades e regras de negócio do **Esfiharia Manager**, servindo como base para os testes manuais de QA.

## 2. Escopo funcional identificado

| RF | Módulo | Requisito principal |
|---|---|---|
| RF01 | Login | Autenticar usuários válidos e impedir acesso com credenciais inválidas ou conta inativa. |
| RF02 | Recuperação de senha | Permitir solicitação e redefinição segura da senha. |
| RF03 | Perfis e permissões | Restringir menus e ações conforme o perfil autenticado. |
| RF04 | Usuários | Cadastrar, consultar, editar e ativar/inativar usuários. |
| RF05 | Clientes | Cadastrar, pesquisar, editar, bloquear e desbloquear clientes. |
| RF06 | Insumos e estoque | Controlar insumos, unidades, saldo e estoque mínimo. |
| RF07 | Produtos e receitas | Cadastrar produtos e associar insumos/quantidades às receitas. |
| RF08 | Cardápio | Exibir produtos disponíveis e impedir inclusão de itens indisponíveis. |
| RF09 | Pedidos | Criar pedidos com cliente, itens, atendimento, pagamento e valores corretos. |
| RF10 | Cozinha | Controlar o fluxo Recebido → Produção → Pronto → Entrega. |
| RF11 | Cancelamentos e estornos | Cancelar pedidos e tratar estoque, caixa e destino dos itens conforme a etapa. |
| RF12 | Caixa | Abrir, movimentar, conferir e fechar sessões de caixa com histórico. |
| RF13 | Entregas/Motoboy | Atribuir entregas, permitir confirmação de pagamento e consultar entregas. |
| RF14 | Relatórios | Gerar consultas gerenciais com filtros e dados financeiros/operacionais. |
| RF15 | Impressão | Permitir impressão de pedidos e relatórios em formatos suportados. |
| RF16 | Acompanhamento do pedido | Permitir acompanhamento do pedido por link e invalidá-lo após conclusão. |
| RF17 | Dashboard | Exibir informações e atalhos coerentes com o perfil do usuário. |
| RF18 | Sessão e logout | Encerrar sessão corretamente e impedir reutilização indevida de sessão antiga. |

## 3. Regras de negócio relevantes

- Usuários inativos não devem acessar o sistema.
- Cada perfil deve visualizar apenas funcionalidades autorizadas.
- Um pedido deve possuir os dados obrigatórios antes da confirmação.
- A forma de pagamento deve ser informada conforme a regra do pedido.
- Produtos sem insumos suficientes não devem ser vendidos normalmente.
- O estoque deve ser atualizado no momento definido pelo fluxo da cozinha.
- Pedidos cancelados não devem continuar no fluxo de produção.
- Cancelamentos e estornos devem manter consistência entre pedido, estoque e caixa.
- O caixa deve aceitar apenas uma sessão aberta por vez.
- Sessões antigas devem ser tratadas sem corromper o fechamento atual.
- Valores de venda, entrega, estorno e formas de pagamento devem permanecer rastreáveis nos relatórios.
- O perfil de cozinha não deve alterar dados financeiros.
- O motoboy deve acessar apenas funcionalidades relacionadas às entregas que lhe competem.
- Links sensíveis, como redefinição de senha, devem expirar conforme a regra configurada.
- O sistema deve manter consistência entre frontend, API e banco de dados.

## 4. Requisitos não funcionais a validar

| ID | Categoria | Requisito |
|---|---|---|
| RNF01 | Usabilidade | As telas devem ser compreensíveis e adequadas ao uso durante horários de pico. |
| RNF02 | Segurança | Funcionalidades devem respeitar autenticação e autorização por perfil. |
| RNF03 | Integridade | Operações de pedido, estoque e caixa não devem gerar dados inconsistentes. |
| RNF04 | Desempenho | Buscas, troca de status e cálculos devem responder em tempo aceitável. |
| RNF05 | Compatibilidade | A aplicação deve funcionar nos ambientes web/mobile previstos pelo projeto. |
| RNF06 | Rastreabilidade | Operações relevantes devem manter histórico suficiente para conferência. |
| RNF07 | Validação | Campos obrigatórios e formatos inválidos devem ser tratados antes da gravação. |
| RNF08 | Recuperação | Falhas de operação não devem deixar registros parcialmente processados. |

## 5. Riscos de qualidade

Os pontos de maior risco são os fluxos que integram **pedido + estoque + cozinha + caixa**, pois uma falha pode causar divergência financeira ou de estoque. Também são prioritários os testes de **permissão por perfil**, **cancelamento/estorno**, **sessões de caixa**, **pagamento na entrega**, **recuperação de senha** e **indisponibilidade de produtos**.

## 6. Critério de aprovação geral

A versão será considerada adequada para homologação quando os casos críticos e de alta prioridade estiverem aprovados e não houver bug crítico ou alto sem tratamento.
