<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/ciencia-da-computacao">Ciência da Computação</a></h3>


<font size="+12"><center>
*&lt;Sistema de Presença&gt;*
</center></font>

**Conteúdo**

- [Autores](#autores)
- [Descrição do Projeto](#descricao-do-projeto)
- [Análise de Requisitos Funcionais e Não-Fucionais](#analise-dos-requisitos)
- [Diagrama de Atividades](#diagrama-de-atividades) 
- [Diagrama de Casos de Uso](#diagrama-de-casos-de-uso)
- [Descrição dos Casos de Uso](#descrição-dos-casos-de-uso)
- [Diagrama de Senquencia](#diagrama-de-sequencia)
- [Diagrama de Classes](#diagrama-de-classes)
- [Diagrama de Estados](#diagrama-de-estados)
- [Diagrama de Implementação](#diagrama-de-implementacao)
- [Referências](#referencias)


<a id="autores"></a>
# Autores

* Vitor Alves Pereira - 10410862
* Eduardo Takashi Missaka - 10417877
* Fernando Mathias Ferro dos Santos - 10418683 
* Tiago Silveira Lopes - 10417600

<a id="descricao-do-projeto"></a>
# Descrição do Projeto
Com o intuito de otimizar o sistema de presença da Escola Infinito, desenvolvemos o **Sistema de Presença**, um sistema misto de presença — online e presencial — que agiliza o processo de validação de comparecimento dos alunos nas aulas ministradas durante o ano/semestre, criando uma relação mais assertiva com o controle de faltas e presença com segurança e facilidade no dia-a-dia.

Para isso, o sistema conta com duas fases essenciais: a fase presencial e a fase online. A fase presencial é a fase em que o professor irá chamar os nomes dos alunos no início da aula, um a um, e identificá-los ao sistema, isto é, marcar manualmente a presença de cada um deles. Essa etapa é fundamental para garantir que os alunos chegaram em segurança na classe e que o professor, como o responsável, os viu e garantiu por meio do processo manual de presença que estavam na aula em uma data definida por DD/MM/AA. Tendo realizado esta etapa, a fase online seria a fase a ser realizada em seguida para determinar que os alunos compareceram nas próximas aulas ministradas no dia. Assim, por meio de um aplicativo mobile e/ou web, o professor dispara — por meio do sistema — telas individuais para cada aluno, com uma descrição da aula, dia e horário, identificador único e um botão de presença e, assim, cada aluno registra a sua presença na aula de forma rápida e efetiva, sem que a aula perca muito tempo para esta tarefa.

Contudo, por ser um sistema flexível e acessível a todos, é possível que em casos específicos a presença possa ser marcada manualmente por um responsável na aula ou secretaria da escola, como: **1. Atrasos:** Consideramos que atrasos são parte do cotidiano e por isso o sistema permite que durante a primeira aula seja possível marcar a presença de alunos que chegaram após o horário em um dia DD/MM/AA; **2. Problemas de Saúde:** Se um aluno possui a presença identificada na fase presencial e por motivos de problemas de saúde teve que se ausentar das próximas aulas, o sistema permite que as faltas sejam anuladas por um responsável na secretaria; **3. Dificuldades ao acesso à tecnologia:** No caso de possíveis restrições à tecnologia, seja pelos responsáveis ou acessibilidade, é possível que por meio de um requerimento na secretaria seja autorizado que estes alunos realizem a sua presença sempre de maneira manual, por meio de uma assinatura durante as fases presencial e online.

Sobre o controle de faltas, há um limite estabelecido pela escola que é de no mínimo setenta e cinco por cento (75%) de presença nas aulas do ano para receber a aprovação. Alunos que possuem faltas consecutivas a partir de sete (7) dias receberão uma notificação no aplicativo e seus responsáveis receberão uma notificação via e-mail com o intuito de manter os responsáveis pelos alunos cientes da situação de cada um deles neste contexto. A contabilização das presenças e faltas pode ser acessada por meio do perfil do aluno no aplicativo.

Portanto, o sistema visa otimizar o dia-a-dia dos professores e alunos e facilitar o controle das presenças e faltas durante o período letivo e por isso, acreditamos que o sistema cumpre a tarefa de maneira eficaz e segura. O objetivo do projeto é sempre evoluir e oferecer atualizações para cumprir o que é requerido da melhor maneira possível e por isso futuras atualizações podem vir após o seu lançamento. Isso posto, confira a seguir as especificações técnicas dos processos descritos para esclarecer detalhes de implementação e funcionamento do projeto apresentado.

<a id="analise-dos-requisitos"></a>
# Análise de Requisitos Funcionais e Não-Funcionais
1. **Requisitos Funcionais:**
    - O sistema deve permitir que os professores e alunos obtenham acesso por meio de uma conta única com acesso a funcionalidades restritas de acordo com as predefinições  hierárquicas da instituição;
    - O sistema deve possibilitar que o professor marque a presença de um ou mais alunos manualmente, de acordo com a fase presencial, e disponibilize as telas individuais aos alunos para o cumprimento da fase online;
    - O sistema deve permitir redefinir o estado de presença e/ou falta de qualquer aluno por um professor ou responsável na secretaria por meio de uma aprovação de um requerimento;
    - O sistema deve disponibilizar as telas aos alunos com os dados do professor e disciplina, prédio e classe, dia e horário e botão de confirmação de presença na fase online;
    - O sistema deve permitir que somente o professor possa disponibilizar as telas aos alunos por meio de sua conta privada;
    - O sistema deve garantir que somente seja possível garantir a presença na fase online se e somente se a fase presencial for realizada anteriormente.
2. **Requisitos Não-Funcionais:**
    - O sistema deve garantir que a contabilidade das presenças e da relação presença e faltas esteja acessível e funcional para todos os alunos;
    - O sistema deve garantir que após um aluno faltar mais de sete (7) dias consecutivos os pais e responsáveis receberão uma notificação via e-mail e o aluno em questão receberá uma notificação em seu aplicativo com acesso a sua conta privada;
    - O sistema deve garantir a segurança dos dados dos alunos, professores e secretaria por meio de estratégias de segurança de dados, como a criptografia;
    - O sistema deve ser acessível em dispositivos móveis e desktops por meio de uma aplicação web e mobile.

<a id="diagrama-das-atividades"></a>
# Diagrama de Atividades

| Fase Presencial | Fase Online |
| -------- | -------- |
| <img src="/docs/Fase Presencial.jpeg" alt="Fase Presencial"/> | <img src="/docs/Fase Online.jpeg" alt="Fase Online"/> |


<a id="diagrama-dos-casos-de-uso"></a>
# Diagrama de Casos de Uso
<img src="/docs/Diagrama dos Casos de Uso.jpg" alt="Diagrama dos Casos de Uso"/>

<a id="descricao-dos-casos-de-uso"></a>
# Descrição dos Casos de Uso
## Descrição dos Requisitos
Refere-se a quais requisitos funcionais o caso de uso está associado. Nesse caso, destacam-se:

- RF1: O sistema deve permitir que os professores e alunos obtenham acesso por meio de uma conta única com acesso a funcionalidades restritas de acordo com as predefinições hierárquicas da instituição;
- RF2:  O sistema deve possibilitar que o professor marque a presença de um ou mais alunos manualmente, de acordo com a fase presencial, e disponibilize as telas individuais aos alunos para o cumprimento da fase online;
- RF3: O sistema deve permitir redefinir o estado de presença e/ou falta de qualquer aluno por um professor ou responsável na secretaria por meio de uma aprovação de um requerimento;
- RF4: O sistema deve disponibilizar as telas aos alunos com os dados do professor e disciplina, prédio e classe, dia e horário e botão de confirmação de presença na fase online;
- RF5: O sistema deve permitir que somente o professor possa disponibilizar as telas aos alunos por meio de sua conta privada;
- RF6: O sistema deve garantir que somente seja possível garantir a presença na fase online se e somente se a fase presencial for realizada anteriormente.

## Especificação dos Casos de Uso do Projeto
### Sistema de Presenças
| **Sistema**                  | **Descrição**                                                                                                                                          |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Função**                   | Fazer registro da frequência de todos os alunos matriculados numa instituição durante semestre/bimestre/ano.                                           |
| **Descrição**                | Sistema de presença que registra aula por aula a frequência de todos os alunos. Alunos e professores interagem para confirmar presença.                  |
| **Entradas**                 | Registro por parte de professores da chamada dos alunos em sala de aula e confirmação dos alunos de sua presença posteriormente.                         |
| **Fonte**                    | Indivíduos que interagem com o sistema.                                                                                                              |
| **Saídas**                   | Para cada aula, a saída deve ser uma lista com o registro de presença da turma.                                                                        |
| **Destino**                  | Banco de dados de presenças.                                                                                                                         |
| **Ação**                     | O sistema valida o aluno e registra a presença correspondente na turma correta.                                                                        |
| **Requer**                   | O aluno deve estar autenticado e a presença deve ter sido liberada pelo professor.                                                                     |
| **Pré-Condição**             | O professor deve ter liberado o período de registro de presença para a aula específica.                                                                |
| **Pós-Condição**             | A presença do aluno é registrada no sistema, disponível para revisão pelo professor.                                                                    |
| **Efeitos Colaterais**      | O aluno que não realizar o registro dentro do período permitido será marcado como ausente.                                                             |

### Especificação dos Casos de Uso para cada RF
| **Ator Principal**            | Administrador do sistema                                                                 |
|------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Atores Secundários**        | Professores e alunos                                                                      |
| **Resumo**                    | Usuários do sistema devem acessar suas contas vinculadas à instituição de forma prática.  |
| **Pré-Condições**             | O administrador deve estar autenticado no sistema e ter permissões de gerenciamento de contas. |
| **Pós-Condições**             | O sistema criará, atualizará ou removerá as contas de usuários conforme as ações executadas. |
| **Fluxos Principais**         | **Ação do Cliente (Administrador)**                                                     |
|                               | 1. Acessa o sistema e autentica-se.                                                     |
|                               | 2. Seleciona a opção de "Gerenciar Contas de Usuários".                                  |
|                               | 3. Escolhe criar, atualizar ou excluir uma conta.                                        |
|                               | **Ação do Sistema**                                                                      |
|                               | 1. Valida os dados e realiza a ação solicitada.                                          |
|                               | 2. Confirma a ação e o administrador recebe uma notificação.                             |
| **Fluxo Alternativo**         | Se o administrador precisar pesquisar contas antes de executar alguma ação, ele pode usar a função de busca por nome, e-mail ou ID do usuário antes de criar, editar ou excluir contas. |
| **Fluxos de Exceção**         | Caso o administrador insira dados inválidos ou incompletos, o sistema exibe uma mensagem de erro e solicita a correção dos dados. |
| **Restrições e Validações**   | 1. O administrador deve estar autenticado e ter privilégios para gerenciar contas de usuários. |
|                               | 2. O sistema deve garantir a unicidade de e-mails para criação de novas contas.          |
|                               | 3. Dados obrigatórios devem ser validados antes da criação ou atualização.               |
|                               | 4. Contas de professores não podem ser excluídas se estiverem vinculadas a turmas ativas ou registros de presença. |

### RF2: Liberar Registro de Presença
| **Ator Principal**            | Administrador do sistema                                                                 |
|-------------------------------|------------------------------------------------------------------------------------------|
| **Atores Secundários**        | Professores e alunos                                                                      |
| **Resumo**                    | Usuários do sistema devem acessar suas contas vinculadas à instituição de forma prática.  |
| **Pré-Condições**             | O administrador deve estar autenticado no sistema e ter permissões de gerenciamento de contas. |
| **Pós-Condições**             | O sistema criará, atualizará ou removerá as contas de usuários conforme as ações executadas. |
| **Fluxos Principais**         | **Ação do Cliente (Administrador)**                                                     |
|                               | 1. Acessa o sistema e autentica-se.                                                     |
|                               | 2. Seleciona a opção de "Gerenciar Contas de Usuários".                                  |
|                               | 3. Escolhe criar, atualizar ou excluir uma conta.                                        |
|                               | **Ação do Sistema**                                                                      |
|                               | 1. Valida os dados e realiza a ação solicitada.                                          |
|                               | 2. Confirma a ação e o administrador recebe uma notificação.                             |
| **Fluxo Alternativo**         | Se o administrador precisar pesquisar contas antes de executar alguma ação, ele pode usar a função de busca por nome, e-mail ou ID do usuário antes de criar, editar ou excluir contas. |
| **Fluxos de Exceção**         | Caso o administrador insira dados inválidos ou incompletos, o sistema exibe uma mensagem de erro e solicita a correção dos dados. |
| **Restrições e Validações**   | 1. O administrador deve estar autenticado e ter privilégios para gerenciar contas de usuários. |
|                               | 2. O sistema deve garantir a unicidade de e-mails para criação de novas contas.          |
|                               | 3. Dados obrigatórios devem ser validados antes da criação ou atualização.               |
|                               | 4. Contas de professores não podem ser excluídas se estiverem vinculadas a turmas ativas ou registros de presença. |

### RF3: Secretaria reverter/modificar presenças ou faltas
| **Ator Principal**            | Administrador (secretaria), sistema                                                     |
|-------------------------------|------------------------------------------------------------------------------------------|
| **Atores Secundários**        | Aluno                                                                                    |
| **Resumo**                    | O sistema deve permitir redefinir o estado de presença e/ou falta de um aluno pelo administrador do sistema. |
| **Pré-Condições**             | Administrador do sistema deve ter acesso e capacidade de modificar todo o banco de dados do registro de presença. |
| **Pós-Condições**             | Faltas devem ser anuladas (ou revertidas para presença) no sistema após modificação feita pelo administrador no(s) banco(s) de dados específico(s). |
| **Fluxos Principais**         | **Ação do Cliente (Administrador)**                                                     |
|                               | 1. Se autentica no sistema.                                                             |
|                               | 2. Acessa e modifica no sistema os bancos de dados do registro de presença relacionados ao requerimento. |
|                               | 3. Registra e salva as alterações feitas pelo administrador.                             |
| **Fluxo Alternativo**         | Se a secretaria precisar de mais informações do aluno para processar o requerimento, ela pode contatá-lo por e-mail ou telefone antes de tomar uma decisão. |
| **Fluxos de Exceção**         | Se o requerimento não contiver informações suficientes ou não for assinado, a secretaria rejeita o requerimento e notifica o aluno para que ele forneça as informações necessárias. |
| **Restrições e Validações**   | 1. A secretaria deve estar autenticada e ter permissões para modificar registros de presença. |
|                               | 2. O sistema deve verificar se o registro de presença ou falta existe antes de permitir a modificação. |
|                               | 3. O requerimento deve estar em conformidade com as políticas da instituição, que podem incluir prazos para submissão e justificativas necessárias. |

### RF4: Disponibilizar Tela de Registro de Presença Online
| **Ator Principal**            | Aluno                                                                                    |
|-------------------------------|------------------------------------------------------------------------------------------|
| **Atores Secundários**        | Professor, Sistema                                                                       |
| **Resumo**                    | O sistema deve exibir uma interface para os alunos, contendo os dados do professor, disciplina, prédio e classe, dia e horário da aula, além de um botão para confirmação de presença. |
| **Pré-Condições**             | O aluno deve estar autenticado no sistema e a aula deve estar liberada para registro de presença pelo professor. |
| **Pós-Condições**             | O aluno visualiza as informações da aula e pode registrar sua presença.                  |
| **Fluxos Principais**         | **Ação do Cliente (Aluno)**                                                             |
|                               | 1. Acessa o sistema e realiza o login.                                                  |
|                               | 2. Seleciona a aula que deseja registrar a presença.                                    |
|                               | **Ação do Sistema**                                                                      |
|                               | 1. Apresenta ao aluno uma lista de aulas disponíveis para registro de presença, se existirem. |
|                               | 2. Exibe os seguintes dados na tela: Professor, disciplina, prédio, sala, dia e horário. |
|                               | 3. Registra no sistema após o aluno confirmar presença.                                   |
| **Fluxo Alternativo**         | Se não houver aulas programadas para o dia, o sistema informa ao aluno que não há aulas disponíveis para registro de presença. |
| **Fluxos de Exceção**         | Aluno tenta registrar presença fora do período liberado pelo professor. O sistema deve exibir mensagem de erro. |
| **Restrições e Validações**   | 1. O aluno deve estar autenticado para visualizar a tela de registro de presença.        |
|                               | 2. A aula deve estar ativada e liberada para registro de presença pelo professor.        |
|                               | 3. O sistema deve garantir que a informação exibida esteja atualizada e correta, refletindo as configurações da aula no momento do registro. |

### RF5: Disponibilizar telas somente pelo professor
| **Ator Principal**            | Professor                                                                                |
|-------------------------------|------------------------------------------------------------------------------------------|
| **Atores Secundários**        | Aluno, Sistema                                                                          |
| **Resumo**                    | Somente o professor, utilizando sua conta privada, pode liberar a tela de registro de presença para os alunos, permitindo que eles confirmem a presença nas aulas. |
| **Pré-Condições**             | O professor deve estar autenticado no sistema e a aula deve estar registrada corretamente no sistema. |
| **Pós-Condições**             | A tela de registro de presença é liberada para os alunos vinculados à aula selecionada pelo professor. |
| **Fluxos Principais**         | **Ação do Cliente (Professor)**                                                         |
|                               | 1. Faz login em sua conta privada.                                                      |
|                               | 2. Acessa a aula específica que deseja liberar presenças.                              |
|                               | **Ação do Sistema**                                                                      |
|                               | 1. Exibe detalhes da aula como prédio, turma, data e horário.                          |
|                               | 2. Sistema ativa a funcionalidade de registro de presença para os alunos daquela turma e envia notificação para os mesmos. |
| **Fluxo Alternativo**         | Se o professor tentar liberar a presença fora do horário da aula, o sistema exibe uma mensagem de aviso informando que a liberação não é permitida. |
| **Fluxos de Exceção**         | Caso o professor tente liberar a presença para uma aula que não está cadastrada ou com dados incorretos, o sistema exibe um erro e não permite a liberação. |
| **Restrições e Validações**   | 1. Apenas o professor ou administrador pode liberar a tela de registro de presença.      |
|                               | 2. O sistema deve garantir que a conta do professor seja válida e que ele esteja vinculado à aula selecionada. |
|                               | 3. O professor só pode liberar o registro de presença no período de tempo específico definido pela instituição. |

### RF6: Garantir Presença na Fase Online Somente Após Fase Presencial
| **Ator Principal**            | Aluno                                                                                    |
|-------------------------------|------------------------------------------------------------------------------------------|
| **Atores Secundários**        | Professor, Sistema                                                                       |
| **Resumo**                    | O sistema deve garantir que o aluno possa registrar sua presença na fase online somente se a fase presencial da aula tiver sido realizada e registrada pelo professor. |
| **Pré-Condições**             | A fase presencial da aula deve ter sido realizada e a presença do aluno deve ter sido registrada pelo professor. |
| **Pós-Condições**             | O aluno poderá registrar a presença na fase online, caso tenha comparecido e sido registrado na fase presencial. |
| **Fluxos Principais**         | **Ação do Cliente (Aluno)**                                                             |
|                               | 1. Acessa o sistema para realizar o registro de presença na fase online.                 |
|                               | **Ação do Sistema**                                                                      |
|                               | 1. Verifica se a fase presencial foi realizada e se o aluno teve presença confirmada, liberando a tela caso sim. |
|                               | 2. Confirma sua presença na fase online.                                                |
| **Fluxo Alternativo**         | Se o aluno tentar acessar a fase online antes da realização da fase presencial, o sistema bloqueia o acesso à tela de registro de presença. |
| **Fluxos de Exceção**         | Se o aluno tentar acessar a tela de presença fora do horário de aula.                   |
| **Restrições e Validações**   | 1. A presença na fase online só pode ser registrada se a fase presencial tiver sido realizada. |
|                               | 2. O sistema deve garantir a correspondência entre a fase presencial e a fase online da mesma aula, evitando possíveis erros. |


<a id="diagrama-de-sequencia"></a>
# Diagrama de Sequência
*&lt;Diagrama de ordem e interação dos objetos&gt;*

<a id="diagrama-de-classes"></a>
# Diagrama de Classes

*&lt;Diagrama de relacionamento entre classes para os seus atributos e operações&gt;*

<a id="diagrama-de-estados"></a>
# Diagrama de Estados

*&lt;Diagrama para permite modelar o comportamento interno de um determinado objeto, subsistema ou sistema global&gt;*

<a id="diagrama-de-implementacao"></a>
# Diagrama de Implantação

*&lt;Diagrama para exibir o relacionamento de hardware e software no projeto&gt;*

<a id="referencias"></a>
# Referências

*&lt;Lista de referências&gt;*
