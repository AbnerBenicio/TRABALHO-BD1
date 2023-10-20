# TRABALHO 01:  Título do Trabalho

Trabalho desenvolvido durante a disciplina de BD1

# Sumário

### 1. COMPONENTES<br>

Integrantes do grupo<br>
Abner Benicio: abnerbeniciosilva123@gmail.com<br>
Pedro Henrique: pedrohtbernabe@gmail.com<br>
Pedro Lucas: pedroluxa871632@gmail.com<br>
Vinícius Caetano: viniciusgcaetano@hotmail.com<br>
<br>

### 2.MINI-MUNDO<br>

Descrever o mini-mundo! (Não deve ser maior do que 30 linhas, se necessário resumir para justar) <br>
Entrevista com o usuário e identificação dos requisitos.(quando for o caso de sistemas com cliente  real)<br>
Descrição textual das regras de negócio definidas como um  subconjunto do mundo real 
cujos elementos são propriedades que desejamos incluir, processar, armazenar, 
gerenciar, atualizar, e que descrevem a proposta/solução a ser desenvolvida.

>	Uma plataforma de tutoria busca reunir pessoas qualificadas em uma ampla variedade de assuntos e aquelas que desejam se especializar nesses temas. Para atingir esse objetivo, a plataforma precisa de um sistema que possa agrupar essas pessoas em salas de tutoria, onde poderão colaborar e se ajudar mutuamente durante o período de tutoria. Além disso, os tutores devem ser capazes de disponibilizar conteúdo para os alunos, e todos os participantes devem poder se comunicar por meio de um chat de texto, áudio e vídeo.<br>
	Para isso, cada usuário deverá ter: ID, nome, e-mail, telefone e senha. Dentro dos usuários,  teremos  funcionários, que terão os mesmos atributos de usuários, além de matrícula e salário.<br>
	Em relação aos temas, cada tema da plataforma deverá ter um ID, descrição e categoria à qual esse tema pertence. As salas criadas deverão também conter um ID, aluno, tutor e tema abordado na sala, além de material complementar disponibilizado, se houver.<br>
	Além disso, a plataforma terá um acervo público, onde os próprios usuários vão poder alimentá-lo com publicações. Os conteúdos publicados deverão ser curados por usuários administradores da plataforma, que são os funcionários. Cada publicação deve ter um ID próprio, seu autor e tema abordado.<br>
	Por fim, haverá também uma loja onde os usuários poderão trocar pontos, obtidos ao ministrar tutoria e publicar no acervo da plataforma, por brindes. Sendo assim, cada produto deverá ter um ID, nome e valor.

### 3.PERGUNTAS A SEREM RESPONDIDAS<br>

#### 3.1 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO?

    a) O sistema proposto poderá fornecer quais tipos de relatórios e informaçes? 
    b) Crie uma lista com os 5 principais relatórios que poderão ser obtidos por meio do sistema proposto!

a) O sistema poderá fornecer informações sobre as pessoas cadastradas, suas participações como tutores/tutorados, informações sobre os assuntos mais pedidos pelos alunos, relatórios sobre o andamento da loja interna do sistema e também acerca do acervo disponibilizado.

b)

1. Uso do sistema (tutores e tutorados)

2. Assuntos mais pedidos

3. Materiais no acervo

4. Pessoas e seus assuntos de conhecimento

5. Situação de uma pessoa na loja virtual

### 5.MODELO CONCEITUAL<br>

    A) Utilizar a Notação adequada (Preferencialmente utilizar o BR Modelo 3)
    B) O mínimo de entidades do modelo conceitual pare este trabalho será igual a 3 e o Máximo 5.
        * informe quais são as 3 principais entidades do sistema em densenvolvimento<br>(se houverem mais de 3 entidades, pense na importância da entidade para o sistema)       
    C) Principais fluxos de informação/entidades do sistema (mínimo 3). <br>Dica: normalmente estes fluxos estão associados as tabelas que conterão maior quantidade de dados 
    D) Qualidade e Clareza
        Garantir que a semântica dos atributos seja clara no esquema (nomes coerentes com os dados).
        Criar o esquema de forma a garantir a redução de informação redundante, possibilidade de valores null, 
        e tuplas falsas (Aplicar os conceitos de normalização abordados).   

![image](https://github.com/AbnerBenicio/TRABALHO-BD1/assets/112874576/5f7059d3-f0b7-42d7-a236-7468e74a5762)
)

#### 5.1 Validação do Modelo Conceitual

    [Grupo01]: Filipe Moura, João Pedro Spinassé, Marlon Ribeiro e Samuel Ferreira
    [Grupo02]: Arthur Cremasco, Bruno Mian e Thalison Vinícius
#### 5.2 Descrição dos dados

    [objeto]: [descrição do objeto]
    
    EXEMPLO:
    CLIENTE: Tabela que armazena as informações relativas ao cliente<br>
    CPF: campo que armazena o número de Cadastro de Pessoa Física para cada cliente da empresa.<br>

**USUÁRIO:** Tabela que contém informações sobre os usuários da plataforma.  
- *id:* Campo que armazena um identificador único para cada usuário na plataforma.  
- *nome:* Campo que guarda o nome do usuário.  
- *email:* Campo que armazena o endereço de e-mail associado ao usuário.  
- *senha:* Campo que contém a senha de acesso do usuário.



**FUNCIONÁRIO:** Subtabela que herda os atributos da tabela USUÁRIO e adiciona informações específicas para funcionários.  
- *matricula:* Campo que registra a matrícula única de cada funcionário na plataforma.  
- *salario:* Campo que armazena o salário do funcionário.

**TEMA:** Tabela que contém informações sobre os temas disponíveis na plataforma.  
- *id:* Campo que armazena um identificador único para cada tema.  
- *descricao:* Campo que guarda a descrição do tema.  

**SALA:** Tabela que registra informações sobre as salas de tutoria criadas.  
- *id:* Campo que armazena um identificador único para cada sala.  

**ARTIGO:** Tabela que guarda informações sobre o artigo que é publicado por um aluno/tutor.  
- *id:* Campo que armazena um identificador único para cada artigo.  
- *titulo:* Campo que referencia o título do artigo.
- *descricao:* Campo que armazena a descrição do artigo .  

**CATEGORIA:** Tabela que armazena informações sobre a categoria de um tema.  
- *id:* Campo que armazena um identificador único para cada publicação.  
- *descricao:* Campo que referencia a descrição da categoria.  



    

> # Marco de Entrega 01: Do item 1 até o item 5.2 (5 PTS) <br>

### 6    MODELO LÓGICO<br>

        a) inclusão do esquema lógico do banco de dados
        b) verificação de correspondencia com o modelo conceitual 
        (não serão aceitos modelos que não estejam em conformidade)

 ![logico_trabalho_img](https://github.com/AbnerBenicio/TRABALHO-BD1/assets/112874576/b50c8e42-d443-4280-8ce0-2654684f253e)


### 7    MODELO FÍSICO<br>

        a) inclusão das instruções de criacão das estruturas em SQL/DDL 
        (criação de tabelas, alterações, etc..) 

### 8    INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>

        a) Script das instruções relativas a inclusão de dados 
    Requisito mínimo: (Script dev conter: Drop para exclusão de tabelas + create definição de para tabelas e estruturas de dados + insert para dados a serem inseridos)
        OBS
    1) Criar um novo banco de dados para testar a restauracao (em caso de falha na restauração o grupo não pontuará neste quesito)
        2) script deve ser incluso no template em um arquivo no formato .SQL

### 9    TABELAS E PRINCIPAIS CONSULTAS<br>

    OBS: Usa template da disciplina disponibilizado no Colab.<br>

#### 9.1    CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>

#### 9.2    CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>

#### 9.3    CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)

    a) Criar 5 consultas que envolvam os operadores lógicos AND, OR e Not
    b) Criar no mínimo 3 consultas com operadores aritméticos 
    c) Criar no mínimo 3 consultas com operação de renomear nomes de campos ou tabelas

#### 9.4    CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>

    a) Criar outras 5 consultas que envolvam like ou ilike
    b) Criar uma consulta para cada tipo de função data apresentada.

> # Marco de Entrega 02: Do item 6. até o item 9.1 (5 PTS) <br>

#### 9.5    INSTRUÇÕES APLICANDO ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>

    a) Criar minimo 3 de exclusão
    b) Criar minimo 3 de atualização

#### 9.6    CONSULTAS COM INNER JOIN E ORDER BY (Mínimo 6)<br>

    a) Uma junção que envolva todas as tabelas possuindo no mínimo 2 registros no resultado
    b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho

#### 9.7    CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO (Mínimo 6)<br>

    a) Criar minimo 2 envolvendo algum tipo de junção

#### 9.8    CONSULTAS COM LEFT, RIGHT E FULL JOIN (Mínimo 4)<br>

    a) Criar minimo 1 de cada tipo

#### 9.9    CONSULTAS COM SELF JOIN E VIEW (Mínimo 6)<br>

        a) Uma junção que envolva Self Join (caso não ocorra na base justificar e substituir por uma view)
        b) Outras junções com views que o grupo considere como sendo de relevante importância para o trabalho

#### 9.10    SUBCONSULTAS (Mínimo 4)<br>

     a) Criar minimo 1 envolvendo GROUP BY
     b) Criar minimo 1 envolvendo algum tipo de junção

> # Marco de Entrega 03: Do item 9.2 até o ítem 9.10 (10 PTS)<br>

### 10 RELATÓRIOS E GRÁFICOS

#### a) análises e resultados provenientes do banco de dados desenvolvido (usar modelo disponível)

#### b) link com exemplo de relatórios será disponiblizado pelo professor no AVA

#### OBS: Esta é uma atividade de grande relevância no contexto do trabalho. Mantenha o foco nos 5 principais relatórios/resultados visando obter o melhor resultado possível.

### 11    AJUSTES DA DOCUMENTAÇÃO, CRIAÇÃO DOS SLIDES E VÍDEO PARA APRESENTAÇAO FINAL <br>

#### a) Modelo (pecha kucha)<br>

#### b) Tempo de apresentação 6:40

> # Marco de Entrega 04: Itens 10 e 11 (20 PTS) <br>
> 
> <br>
> <br>

### 12 FORMATACAO NO GIT:<br>

https://help.github.com/articles/basic-writing-and-formatting-syntax/
<comentario no git>

##### About Formatting

    https://help.github.com/articles/about-writing-and-formatting-on-github/

##### Basic Formatting in Git

    https://help.github.com/articles/basic-writing-and-formatting-syntax/#referencing-issues-and-pull-requests

##### Working with advanced formatting

    https://help.github.com/articles/working-with-advanced-formatting/

#### Mastering Markdown

    https://guides.github.com/features/mastering-markdown/

### OBSERVAÇÕES IMPORTANTES

#### Todos os arquivos que fazem parte do projeto (Imagens, pdfs, arquivos fonte, etc..), devem estar presentes no GIT. Os arquivos do projeto vigente não devem ser armazenados em quaisquer outras plataformas.

1. <strong>Caso existam arquivos com conteúdos sigilosos<strong>, comunicar o professor que definirá em conjunto com o grupo a melhor forma de armazenamento do arquivo.

#### Todos os grupos deverão fazer Fork deste repositório e dar permissões administrativas ao usuário do git "profmoisesomena", para acompanhamento do trabalho.

#### Os usuários criados no GIT devem possuir o nome de identificação do aluno (não serão aceitos nomes como Eu123, meuprojeto, pro456, etc). Em caso de dúvida comunicar o professor.

Link para BrModelo:<br>
http://www.sis4.com/brModelo/download.html
<br>

Link para curso de GIT<br>
![https://www.youtube.com/curso_git](https://www.youtube.com/playlist?list=PLo7sFyCeiGUdIyEmHdfbuD2eR4XPDqnN2?raw=true "Title")
