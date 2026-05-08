Este guia foi reestruturado para servir como um **Manual de Referência Técnica de UI/UX** para o time de desenvolvimento. O objetivo é padronizar a interpretação das User Stories e garantir que a fidelidade visual e funcional seja mantida durante a Sprint 3.

* * *

📘 Guia de Referência de UI/UX – Sprint 3 (SwiftPlan)
=====================================================

> **Nota Técnica:** As interfaces apresentadas são protótipos funcionais. O design final deve seguir os padrões de acessibilidade, entretanto a paleta de cores definida é alterável, mas a lógica de componentes descrita abaixo é **mandatória** para o critério de aceitação das tarefas.

* * *

1. Gestão de Atribuições (Visão Coordenador)

--------------------------------------------

**Objetivo:** Alocação de carga horária para docentes com validação de conflitos.

_(Referência: Exemplar de atribuicao.png / Exemplar de atribuicao com erro.png)

[![Ver imagem ampliada](docs/sprint/Sprint-3/img/coord_atribui.png)](docs/sprint/Sprint-3/img/coord_atribui.png)

* **Interatividade:** O uso de _Checkboxes_ permite a seleção múltipla de horários/dias.

* **Tratamento de Conflitos:** Células com **borda vermelha** indicam indisponibilidade (horário já ocupado em outra atribuição).

* **Feedback de Erro:** Caso o usuário tente salvar um conflito, o sistema deve exibir a mensagem de alerta em destaque: _"Atenção: Há horários com conflito selecionados!"_.

* * *

2. Planejamento e Estatísticas (Visão Professor)

------------------------------------------------

**Objetivo:** Acompanhamento de cronograma e métricas de desempenho da disciplina.

_(Referência: Exemplar tela planejamento professor.png)_

* **Navegação Hierárquica:** À esquerda, o cronograma utiliza um componente de _Tree View_ (árvore) por datas.

* **Dashboard de Métricas:** À direita, o sistema deve renderizar estatísticas em tempo real, incluindo gráficos de rosca para status de aulas (Ministradas, Pendentes, Canceladas) e barras de progresso para a Carga Horária (CH).

* * *

3. Monitoramento de Planejamento (Visão Coordenador)

----------------------------------------------------

**Objetivo:** Supervisão das atividades dos professores subordinados.

_(Referência: Exemplar visualizacao planejamento por coord.png)_

* **Filtro de Hierarquia:** O painel esquerdo exibe apenas os professores sob gestão do coordenador logado.

* **Padronização Visual:** A visualização à direita deve ser um "espelho" da visão do professor, garantindo que o coordenador veja exatamente os mesmos dados.

* **Destaque de Status (Cores de Texto):**
  
  * **Amarelo:** Aulas Pendentes.
  
  * **Vermelho:** Aulas Canceladas.
  
  * **Verde:** Aulas Lecionadas.

* * *

4. Gestão de Disciplinas e Cursos

---------------------------------

**Objetivo:** CRUD (Criação, Leitura, Atualização e Exclusão) de entidades acadêmicas.

_(Referência: Exemplar visualizacao disciplinas por coord.png / Exemplar base adm_curso_horarios adicao.png)_

* **Layout Adaptável:** A tabela de listagem ocupa a tela inteira por padrão. O formulário de cadastro (à direita) é **condicional** e só aparece ao clicar em "+ Nova".

* **Ações In-line:** Cada linha deve conter botões de edição e exclusão.

* **Segurança de Dados:** A exclusão exige obrigatoriamente um modal de confirmação (Pop-up) para evitar perda acidental de dados. _(Ref: Exemplar visualizacao disciplinas_exclusao por coord.png)_

* * *

5. Calendário Acadêmico e Bloqueios (Visão Administrador)

---------------------------------------------------------

**Objetivo:** Gestão de feriados, recessos e bloqueios de turnos.

_(Referência: Exemplar bloqueio por adm.png / Exemplar de cadastro de Sprints adm.png)_

* **Lógica de Seleção de Datas:**
  
  1. O usuário seleciona o mês;
  
  2. O grid de dias é gerado dinamicamente;
  
  3. Selecionar um dia abre o painel "Configurar Cancelamento".

* **Hierarquia de Bloqueio:** Se um turno não for especificado, o bloqueio é aplicado ao **dia inteiro**. Se o turno for escolhido, a seleção de horários torna-se **obrigatória**.

* **Legenda de Estados do Calendário:**
  
  * **Vermelho:** Data cancelada/bloqueada.
  
  * **Amarelo:** Seleção atual (ainda não salva).
  
  * **Borda Avermelhada:** Ação de reverter um cancelamento existente.

* * *

6. Layout Estrutural (Shell da Aplicação)

-----------------------------------------

**Objetivo:** Navegação global e contexto de sistema.

_(Referência: Exemplar conexao shell com adm.png)_

* **Header (Topo):** Controles globais de filtragem (Ano/Semestre/Curso) e identificação do usuário com botão de _Logout_.

* **Sidebar (Esquerda):** Menu de navegação por funcionalidades.

* **Banner de Contexto:** Sempre que o usuário visualizar dados históricos (passados), um aviso em destaque deve indicar o **Modo Somente Leitura**.

* * *

7. Configuração de Sprints e Horários

-------------------------------------

**Objetivo:** Definição de prazos e templates de horários.

* **Edição Direta (In-place):** Para as Sprints, as células da tabela devem permitir edição com duplo clique (limitado a 3 linhas fixas).

* **Automação de Horários:** Implementar funções de "Aplicar Template" e "Propagar ao Turno" para otimizar o cadastro em massa de horários de aulas.

* * *

**Equipe de Desenvolvimento:** Em caso de divergência entre a User Story escrita e estas imagens, este guia de UI deve prevalecer como a intenção de design do cliente.
