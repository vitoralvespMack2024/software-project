<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/ciencia-da-computacao">Ciência da Computação</a></h3>


<font size="+12"><center>
*&lt;Nome do Projeto&gt;*
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
Com o intuito de otimizar o sistema de presença da Escola Infinito, desenvolvemos o **Nome do Projeto**, um sistema misto de presença — online e presencial — que agiliza o processo de validação de comparecimento dos alunos nas aulas ministradas durante o ano/semestre, criando uma relação mais assertiva com o controle de faltas e presença com segurança e facilidade no dia-a-dia.

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

*&lt;Diagrama para visualizar o comportamento dos atores&gt;*

<a id="descricao-dos-casos-de-uso"></a>
# Descrição dos Casos de Uso

*&lt;Descrição do comportamento entre os atores/resquisitos&gt;*

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
