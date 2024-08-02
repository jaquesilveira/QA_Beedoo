**Desafio | Analista de Qualidade de Software Júnior**


**ETAPA 1**

Segue abaixo a história de usuário criada para atender o desafio da oportunidade - Analista de Qualidade de Software Júnio na Beedoo.
E para escrita foi levado em consideração a necessidade de **ofertar curso (online e presencias)** para *comercialização* na *Beedoo*, permitindo assim uma maior 
*propagação* e *difusão*.

-------------------------------

**USER STORY - CADASTRO DE CURSO**

**Descrição**
Como um administrador do sistema

eu quero ofertar cursos no portfolio Beedoo 

com o objetivo oferecer cursos presenciais e online de maneira simples e dinâmica.

**Critério de aceitação**

*Critério 01: Acesso ao módulo de cadastro*

Dado que desejo acessar o portfólio de curso da Beedoo

Então deverá apresentar o formulário para inclusão de um novo curso

*Critério 02: Cadastro de curso*

Dado que tenha material de ensino preparado (videoaulas, textos explicativos, atividades, testes e chatbots)

E que tenha um cronograma de ensino (início/fim do curso)

E desejo realizar um cadastro de um novo curso (online ou presencial) para ser ofertado no  portfólio Beedoo

Quando preencher as informações do curso e clicar em cadastrar 

Então deverá apresentar a mensagem em tela “Curso cadastrado com sucesso”

E redirecionar para a listagem de cursos da Beedoo

-------------------------------

**CENÁRIOS E CASO DE TESTE**

Link  Google Doc: [https://docs.google.com/document/d/1i9lRyx-nOxB4cYDlgweCo5fYHImTn_ZtYOF_Fl1zS1M/edit?usp=sharing](https://docs.google.com/document/d/1i9lRyx-nOxB4cYDlgweCo5fYHImTn_ZtYOF_Fl1zS1M/edit)

**CENÁRIO 1	Mostrar mensagem de sucesso quando curso online for criado**
DADO que tenho perfil de administrador

E que esteja acessando o portfólio de curso da Beeboo

E clico em cadastrar

E preencho as informações para  cadastro de curso: Nome, Descrição, instrutor, url, data início/fim, número de vagas, tipo de curso - oline 

QUANDO clico em «Cadastrar Curso»

ENTÃO deverá apresentar a mensagem «Curso cadastrado com sucesso»

E redirecionar para a lista de cursos da Beedoo


**CENÁRIO 2	Mostrar mensagem de sucesso quando curso presencial for criado**

DADO que tenho perfil de administrador

E que esteja acessando o portfólio de curso da Beeboo

E clico em cadastrar

E preencho as informações para  cadastro de curso: Nome, Descrição, instrutor, url, data início/fim, número de vagas, tipo de curso – presencial

QUANDO clico em «Cadastrar Curso»

ENTÃO deverá apresentar a mensagem «Curso cadastrado com sucesso»

E redirecionar para a lista de cursos da Beedoo


**CENÁRIO 3	Não permitir criação de curso com perfil diferente de administrador**

DADO que não tenha perfil de administrador

E que esteja acessando o portfólio de curso da Beeboo

QUANDO clico em cadastrar

ENTÃO não deverá apresentar o formulário de cadastro de curso 


**CENÁRIO 4	Não permitir a inclusão de curso sem preenchimento dos dados de cadastro**

DADO que tenho perfil de administrador

E que esteja acessando o portfólio de curso da Beeboo

E clico em cadastrar

E NÃO preencho as informações para  cadastro de curso: Nome, Descrição, instrutor, url, data início/fim, número de vagas, tipo de curso

QUANDO clico em «Cadastrar Curso»

ENTÃO não deverá incluir o curso sem o preenchimento de dados cadastrais


**CENÁRIO 5	Não permitir a inclusão de curso com data início/fim com períodos retroativos ao dia, mês e ano vigente**
DADO que tenho perfil de administrador

E que esteja acessando o portfólio de curso da Beeboo

E clico em cadastrar

E preencho as informações para  cadastro de curso: Nome, Descrição, instrutor, url, número de vagas, tipo de curso

E preencho data início/fim do curso com dados retroativos ao dia, mês e ano vigente

QUANDO clico em «Cadastrar Curso»

ENTÃO não deverá incluir o curso som data início/fim com dados retroativos ao dia, mês e ano ou data inválida


**CENÁRIO 6	Não permitir a inclusão de curso com data início/fim com períodos retroativos ao dia, mês e ano vigente**
DADO que tenho perfil de administrador

E que esteja acessando o portfólio de curso da Beeboo

E clico em cadastrar

E preencho as informações para  cadastro de curso: Nome, Descrição, instrutor, url, número de vagas, tipo de curso

E preencho data início/fim do curso com dados retroativos ao dia, mês e ano vigente

QUANDO clico em «Cadastrar Curso»

ENTÃO não deverá incluir o curso som data início/fim com dados retroativos ao dia, mês e ano ou data inválida


-------------------------------

**EVIDÊNCIA DOS TESTES**

Link drive: 

-------------------------------

**RELATÓRIO BUGS**

link 
