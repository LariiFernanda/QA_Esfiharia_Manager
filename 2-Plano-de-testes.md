2 — Plano de Testes
1. Identificação
Sistema: Esfiharia Manager  
Tipo de teste: QA manual funcional  
Responsáveis: Equipe do projeto  
Ambiente: Ambiente de desenvolvimento/homologação do Esfiharia Manager
2. Objetivo
Validar se as funcionalidades do sistema atendem aos requisitos esperados, verificando fluxos positivos, negativos, permissões de acesso, validações e integração entre módulos.
3. Escopo
Serão testados:
autenticação e recuperação de senha;
perfis e permissões;
usuários e clientes;
insumos, estoque, produtos e receitas;
cardápio;
pedidos;
cozinha;
cancelamentos e estornos;
caixa;
entregas/motoboy;
relatórios;
impressão;
acompanhamento do pedido;
dashboard;
sessão e logout.
4. Fora do escopo
Testes automatizados de carga, invasão, pentest e auditoria de infraestrutura não fazem parte desta rodada manual, salvo quando solicitados separadamente.
5. Estratégia
Serão utilizados:
testes funcionais;
testes positivos;
testes negativos;
testes de validação de campos;
testes de permissão;
testes de integração entre módulos;
testes básicos de usabilidade;
testes de regressão após correções.
6. Prioridades
Prioridade	Descrição
Crítica	Login, pedidos, estoque, cozinha, caixa, cancelamentos e pagamentos
Alta	Perfis, usuários, clientes, cardápio, motoboy e relatórios
Média	Dashboard, impressão, acompanhamento e recuperação de senha
Baixa	Ajustes visuais que não impedem a operação
7. Dados de teste
Recomenda-se preparar:
usuário Administrador ativo;
usuário Atendente ativo;
usuário Cozinha ativo;
usuário Motoboy ativo;
usuário inativo;
cliente ativo e cliente bloqueado;
produto disponível;
produto com estoque insuficiente;
insumos com saldo normal e abaixo do mínimo;
caixa aberto e caixa fechado;
pedido de retirada;
pedido de entrega;
pedido pago e não pago;
pedido em cada etapa da cozinha.
8. Critérios de entrada
aplicação disponível;
banco de dados acessível;
API funcionando;
usuários de teste cadastrados;
dados mínimos preparados.
9. Critérios de saída
todos os casos críticos executados;
bugs críticos documentados;
evidências anexadas;
relatório final atualizado;
resultado de cada caso marcado como aprovado, reprovado ou bloqueado.
10. Evidências
Cada execução deve possuir, quando aplicável:
print da tela;
vídeo curto do fluxo;
mensagem de erro apresentada;
identificação do usuário/perfil utilizado;
data da execução.
11. Severidade dos bugs
Severidade	Definição
Crítica	Impede operação principal ou causa perda/corrupção de dados
Alta	Função importante falha sem alternativa aceitável
Média	Função falha, mas há contorno
Baixa	Problema visual, textual ou de baixo impacto
12. Fluxo de tratamento
Executar caso de teste.
Registrar resultado.
Se falhar, abrir bug.
Corrigir o sistema.
Retestar o bug.
Executar regressão no fluxo relacionado.
Atualizar o relatório final.
