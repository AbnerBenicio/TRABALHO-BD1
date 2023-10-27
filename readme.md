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

![image](https://github.com/AbnerBenicio/TRABALHO-BD1/assets/112874576/43f52930-e6e9-467a-9699-c9a161a20720)

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

```
BEGIN;


DROP TABLE IF EXISTS public.usuario;

CREATE TABLE IF NOT EXISTS public.usuario
(
    id integer NOT NULL DEFAULT nextval('usuario_id_seq'::regclass),
    nome character varying(80) COLLATE pg_catalog."default",
    email character varying(80) COLLATE pg_catalog."default",
    senha character varying(20) COLLATE pg_catalog."default",
    CONSTRAINT usuario_pkey PRIMARY KEY (id)
);

DROP TABLE IF EXISTS tutoria."ARTIGO";

CREATE TABLE IF NOT EXISTS tutoria."ARTIGO"
(
    id integer NOT NULL DEFAULT nextval('tutoria.artigo_id_seq'::regclass),
    fk_usuario_id integer NOT NULL DEFAULT nextval('tutoria.artigo_fk_usuario_id_seq'::regclass),
    fk_tema_id integer NOT NULL DEFAULT nextval('tutoria.artigo_fk_tema_id_seq'::regclass),
    fk_funcionario_id integer NOT NULL DEFAULT nextval('tutoria.artigo_fk_funcionario_id_seq'::regclass),
    descricao character varying(80) COLLATE pg_catalog."default",
    titulo character varying(10) COLLATE pg_catalog."default" NOT NULL
);

DROP TABLE IF EXISTS tutoria."CATEGORIA";

CREATE TABLE IF NOT EXISTS tutoria."CATEGORIA"
(
    id integer NOT NULL DEFAULT nextval('tutoria.categoria_id_seq'::regclass),
    descricao character varying(50) COLLATE pg_catalog."default",
    CONSTRAINT categoria_pkey PRIMARY KEY (id)
);

DROP TABLE IF EXISTS tutoria."FUNCIONARIO";

CREATE TABLE IF NOT EXISTS tutoria."FUNCIONARIO"
(
    salario double precision,
    id_funcionario integer NOT NULL DEFAULT nextval('tutoria.funcionario_id_funcionario_seq'::regclass),
    fk_usuario_id integer NOT NULL DEFAULT nextval('tutoria.funcionario_fk_usuario_id_seq'::regclass),
    matricula character varying(10) COLLATE pg_catalog."default" NOT NULL,
    CONSTRAINT funcionario_pkey PRIMARY KEY (id_funcionario)
);

DROP TABLE IF EXISTS tutoria."PARTICIPA";

CREATE TABLE IF NOT EXISTS tutoria."PARTICIPA"
(
    id integer NOT NULL DEFAULT nextval('tutoria."PARTICIPA_id_seq"'::regclass),
    fk_sala_id integer NOT NULL DEFAULT nextval('tutoria."PARTICIPA_fk_sala_id_seq"'::regclass),
    fk_usuario_id integer NOT NULL DEFAULT nextval('tutoria."PARTICIPA_fk_usuario_id_seq"'::regclass),
    CONSTRAINT "PARTICIPA_pkey" PRIMARY KEY (id)
);

DROP TABLE IF EXISTS tutoria."SALA";

CREATE TABLE IF NOT EXISTS tutoria."SALA"
(
    id integer NOT NULL DEFAULT nextval('tutoria."SALA_id_seq"'::regclass),
    fk_tema_id integer NOT NULL DEFAULT nextval('tutoria."SALA_fk_tema_id_seq"'::regclass),
    fk_usuario_id integer NOT NULL DEFAULT nextval('tutoria."SALA_fk_usuario_id_seq"'::regclass),
    data_criacao date NOT NULL,
    sts_valida boolean NOT NULL,
    CONSTRAINT "SALA_pkey" PRIMARY KEY (id)
);

DROP TABLE IF EXISTS tutoria."TEMA";

CREATE TABLE IF NOT EXISTS tutoria."TEMA"
(
    id integer NOT NULL DEFAULT nextval('tutoria."TEMA_id_seq"'::regclass),
    fk_categoria_id integer NOT NULL DEFAULT nextval('tutoria."TEMA_fk_categoria_id_seq"'::regclass),
    descricao character varying(50) COLLATE pg_catalog."default",
    CONSTRAINT "TEMA_pkey" PRIMARY KEY (id)
);

DROP TABLE IF EXISTS tutoria."USUARIO";

CREATE TABLE IF NOT EXISTS tutoria."USUARIO"
(
    id integer NOT NULL DEFAULT nextval('tutoria.usuario_id_seq'::regclass),
    nome character varying(80) COLLATE pg_catalog."default" NOT NULL,
    senha character varying(80) COLLATE pg_catalog."default" NOT NULL,
    email character varying(80) COLLATE pg_catalog."default" NOT NULL,
    CONSTRAINT usuario_pkey PRIMARY KEY (id)
);

DROP TABLE IF EXISTS tutoria."USUARIO_TEMA";

CREATE TABLE IF NOT EXISTS tutoria."USUARIO_TEMA"
(
    id integer NOT NULL DEFAULT nextval('tutoria."USUARIO_TEMA_id_seq"'::regclass),
    nivel_conhecimento integer NOT NULL,
    fk_usuario_id integer NOT NULL DEFAULT nextval('tutoria."USUARIO_TEMA_fk_usuario_id_seq"'::regclass),
    fk_tema_id integer NOT NULL DEFAULT nextval('tutoria."USUARIO_TEMA_fk_tema_id_seq"'::regclass),
    CONSTRAINT "USUARIO_TEMA_pkey" PRIMARY KEY (id)
);

ALTER TABLE IF EXISTS tutoria."ARTIGO"
    ADD CONSTRAINT fk_funcionario_id FOREIGN KEY (fk_funcionario_id)
    REFERENCES tutoria."FUNCIONARIO" (id_funcionario) MATCH SIMPLE
    ON UPDATE NO ACTION
    ON DELETE RESTRICT;


ALTER TABLE IF EXISTS tutoria."ARTIGO"
    ADD CONSTRAINT fk_tema_id FOREIGN KEY (fk_tema_id)
    REFERENCES tutoria."TEMA" (id) MATCH SIMPLE
    ON UPDATE NO ACTION
    ON DELETE NO ACTION
    NOT VALID;


ALTER TABLE IF EXISTS tutoria."ARTIGO"
    ADD CONSTRAINT fk_usuario_id FOREIGN KEY (fk_usuario_id)
    REFERENCES tutoria."USUARIO" (id) MATCH SIMPLE
    ON UPDATE NO ACTION
    ON DELETE SET NULL;


ALTER TABLE IF EXISTS tutoria."FUNCIONARIO"
    ADD CONSTRAINT fk_usuario_id FOREIGN KEY (fk_usuario_id)
    REFERENCES tutoria."USUARIO" (id) MATCH SIMPLE
    ON UPDATE NO ACTION
    ON DELETE NO ACTION;


ALTER TABLE IF EXISTS tutoria."PARTICIPA"
    ADD CONSTRAINT fk_tema_id FOREIGN KEY (fk_sala_id)
    REFERENCES tutoria."SALA" (id) MATCH SIMPLE
    ON UPDATE NO ACTION
    ON DELETE NO ACTION
    NOT VALID;


ALTER TABLE IF EXISTS tutoria."PARTICIPA"
    ADD CONSTRAINT fk_usuario_id FOREIGN KEY (fk_usuario_id)
    REFERENCES tutoria."USUARIO" (id) MATCH SIMPLE
    ON UPDATE NO ACTION
    ON DELETE NO ACTION
    NOT VALID;


ALTER TABLE IF EXISTS tutoria."SALA"
    ADD CONSTRAINT fk_tema_id FOREIGN KEY (fk_tema_id)
    REFERENCES tutoria."TEMA" (id) MATCH SIMPLE
    ON UPDATE CASCADE
    ON DELETE CASCADE;


ALTER TABLE IF EXISTS tutoria."TEMA"
    ADD CONSTRAINT fk_categoria_id FOREIGN KEY (fk_categoria_id)
    REFERENCES tutoria."CATEGORIA" (id) MATCH SIMPLE
    ON UPDATE NO ACTION
    ON DELETE RESTRICT;


ALTER TABLE IF EXISTS tutoria."USUARIO_TEMA"
    ADD CONSTRAINT fk_tema_id FOREIGN KEY (fk_tema_id)
    REFERENCES tutoria."TEMA" (id) MATCH SIMPLE
    ON UPDATE NO ACTION
    ON DELETE NO ACTION
    NOT VALID;


ALTER TABLE IF EXISTS tutoria."USUARIO_TEMA"
    ADD CONSTRAINT fk_usuario_id FOREIGN KEY (fk_usuario_id)
    REFERENCES tutoria."USUARIO" (id) MATCH SIMPLE
    ON UPDATE NO ACTION
    ON DELETE NO ACTION;

END;
```

### 8    INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>

        a) Script das instruções relativas a inclusão de dados 
    Requisito mínimo: (Script dev conter: Drop para exclusão de tabelas + create definição de para tabelas e estruturas de dados + insert para dados a serem inseridos)
        OBS
    1) Criar um novo banco de dados para testar a restauracao (em caso de falha na restauração o grupo não pontuará neste quesito)
        2) script deve ser incluso no template em um arquivo no formato .SQL

```
 #INSERT NA TABELA ARTIGO
 -- Artigo 1
INSERT INTO tutoria."ARTIGO" (fk_usuario_id, fk_tema_id, fk_funcionario_id, descricao, titulo)
VALUES (1, 1, 1, 'Este é um artigo sobre álgebra linear.', 'Álg Lin');

-- Artigo 2
INSERT INTO tutoria."ARTIGO" (fk_usuario_id, fk_tema_id, fk_funcionario_id, descricao, titulo)
VALUES (2, 2, 2, 'Neste artigo, abordamos a biologia celular.', 'Bio Cel');

-- Artigo 3
INSERT INTO tutoria."ARTIGO" (fk_usuario_id, fk_tema_id, fk_funcionario_id, descricao, titulo)
VALUES (3, 3, 1, 'A Idade Média foi um período fascinante na história.', 'Idade Méd');

-- Artigo 4
INSERT INTO tutoria."ARTIGO" (fk_usuario_id, fk_tema_id, fk_funcionario_id, descricao, titulo)
VALUES (4, 4, 2, 'Aprenda as técnicas de pintura a óleo neste artigo.', 'Pintura Ól');

-- Artigo 5
INSERT INTO tutoria."ARTIGO" (fk_usuario_id, fk_tema_id, fk_funcionario_id, descricao, titulo)
VALUES (5, 5, 1, 'Descubra as estratégias de marketing de sucesso.', 'Estratégias');

-- Artigo 6
INSERT INTO tutoria."ARTIGO" (fk_usuario_id, fk_tema_id, fk_funcionario_id, descricao, titulo)
VALUES (6, 1, 2, 'Este é um segundo artigo sobre álgebra linear.', 'Álg Lin 2');

-- Artigo 7
INSERT INTO tutoria."ARTIGO" (fk_usuario_id, fk_tema_id, fk_funcionario_id, descricao, titulo)
VALUES (7, 2, 1, 'A biologia celular é um campo em constante evolução.', 'Bio Cel Ev');

-- Artigo 8
INSERT INTO tutoria."ARTIGO" (fk_usuario_id, fk_tema_id, fk_funcionario_id, descricao, titulo)
VALUES (8, 3, 2, 'Saiba mais sobre a história da Segunda Guerra Mundial.', '2ª Guerra');

-- Artigo 9
INSERT INTO tutoria."ARTIGO" (fk_usuario_id, fk_tema_id, fk_funcionario_id, descricao, titulo)
VALUES (9, 4, 1, 'A escultura em argila é uma forma de arte única.', 'Escul Arg');

-- Artigo 10
INSERT INTO tutoria."ARTIGO" (fk_usuario_id, fk_tema_id, fk_funcionario_id, descricao, titulo)
VALUES (10, 5, 2, 'Aprenda idiomas com dicas práticas.', 'Idiomas D');

#INSERT DE PARTICIPAÇÃO DO USUÁRIO NAS SALAS
-- Participação do Usuário 1 em Salas 1, 2 e 3
INSERT INTO tutoria."PARTICIPA" (fk_sala_id, fk_usuario_id)
VALUES (1, 1), (2, 1), (3, 1);

-- Participação do Usuário 2 em Salas 2, 3 e 4
INSERT INTO tutoria."PARTICIPA" (fk_sala_id, fk_usuario_id)
VALUES (2, 2), (3, 2), (4, 2);

-- Participação do Usuário 3 em Salas 3, 4 e 5
INSERT INTO tutoria."PARTICIPA" (fk_sala_id, fk_usuario_id)
VALUES (3, 3), (4, 3), (5, 3);

-- Participação do Usuário 4 em Salas 4 e 5
INSERT INTO tutoria."PARTICIPA" (fk_sala_id, fk_usuario_id)
VALUES (4, 4), (5, 4);

-- Participação do Usuário 5 em Salas 5, 1 e 2
INSERT INTO tutoria."PARTICIPA" (fk_sala_id, fk_usuario_id)
VALUES (5, 5), (1, 5), (2, 5);

-- Participação do Usuário 6 em Salas 6, 7 e 8
INSERT INTO tutoria."PARTICIPA" (fk_sala_id, fk_usuario_id)
VALUES (6, 6), (7, 6), (8, 6);

-- Participação do Usuário 7 em Salas 7, 8 e 9
INSERT INTO tutoria."PARTICIPA" (fk_sala_id, fk_usuario_id)
VALUES (7, 7), (8, 7), (9, 7);

-- Participação do Usuário 8 em Salas 8, 9 e 10
INSERT INTO tutoria."PARTICIPA" (fk_sala_id, fk_usuario_id)
VALUES (8, 8), (9, 8), (10, 8);

-- Participação do Usuário 9 em Salas 9 e 10
INSERT INTO tutoria."PARTICIPA" (fk_sala_id, fk_usuario_id)
VALUES (9, 9), (10, 9);

-- Participação do Usuário 10 em Salas 10, 1 e 2
INSERT INTO tutoria."PARTICIPA" (fk_sala_id, fk_usuario_id)
VALUES (10, 10), (1, 10), (2, 10);

#INSERT DE SALAS

-- Sala 1
INSERT INTO tutoria."SALA" (fk_tema_id, fk_usuario_id, data_criacao, sts_valida)
VALUES (1, 1, '2023-05-10', true);

-- Sala 2
INSERT INTO tutoria."SALA" (fk_tema_id, fk_usuario_id, data_criacao, sts_valida)
VALUES (2, 2, '2023-06-15', true);

-- Sala 3
INSERT INTO tutoria."SALA" (fk_tema_id, fk_usuario_id, data_criacao, sts_valida)
VALUES (3, 3, '2023-07-20', true);

-- Sala 4
INSERT INTO tutoria."SALA" (fk_tema_id, fk_usuario_id, data_criacao, sts_valida)
VALUES (4, 4, '2023-08-25', true);

-- Sala 5
INSERT INTO tutoria."SALA" (fk_tema_id, fk_usuario_id, data_criacao, sts_valida)
VALUES (5, 5, '2023-09-23', true);

-- Sala 6
INSERT INTO tutoria."SALA" (fk_tema_id, fk_usuario_id, data_criacao, sts_valida)
VALUES (1, 6, '2023-05-15', true);

-- Sala 7
INSERT INTO tutoria."SALA" (fk_tema_id, fk_usuario_id, data_criacao, sts_valida)
VALUES (2, 7, '2023-06-20', true);

-- Sala 8
INSERT INTO tutoria."SALA" (fk_tema_id, fk_usuario_id, data_criacao, sts_valida)
VALUES (3, 8, '2023-07-25', true);

-- Sala 9
INSERT INTO tutoria."SALA" (fk_tema_id, fk_usuario_id, data_criacao, sts_valida)
VALUES (4, 9, '2023-08-30', true);

-- Sala 10
INSERT INTO tutoria."SALA" (fk_tema_id, fk_usuario_id, data_criacao, sts_valida)
VALUES (5, 10, '2023-09-15', true);

#INSERT DE USUÁRIOS

-- Usuário 1
INSERT INTO tutoria."USUARIO_TEMA" (nivel_conhecimento, fk_usuario_id, fk_tema_id)
VALUES (2, 1, 1), (3, 1, 2), (1, 1, 3), (4, 1, 4), (2, 1, 5);

-- Usuário 2
INSERT INTO tutoria."USUARIO_TEMA" (nivel_conhecimento, fk_usuario_id, fk_tema_id)
VALUES (3, 2, 1), (2, 2, 2), (1, 2, 3), (4, 2, 4), (3, 2, 5);

-- Usuário 3
INSERT INTO tutoria."USUARIO_TEMA" (nivel_conhecimento, fk_usuario_id, fk_tema_id)
VALUES (1, 3, 1), (4, 3, 2), (2, 3, 3), (3, 3, 4), (1, 3, 5);

-- Usuário 4
INSERT INTO tutoria."USUARIO_TEMA" (nivel_conhecimento, fk_usuario_id, fk_tema_id)
VALUES (4, 4, 1), (3, 4, 2), (2, 4, 3), (1, 4, 4), (4, 4, 5);

-- Usuário 5 (Adicione instruções para os outros usuários)
INSERT INTO tutoria."USUARIO_TEMA" (nivel_conhecimento, fk_usuario_id, fk_tema_id)
VALUES (3, 5, 1), (2, 5, 2), (1, 5, 3), (4, 5, 4), (3, 5, 5);

-- Usuário 6
INSERT INTO tutoria."USUARIO_TEMA" (nivel_conhecimento, fk_usuario_id, fk_tema_id)
VALUES (1, 6, 1), (4, 6, 2), (2, 6, 3), (3, 6, 4), (1, 6, 5);

-- Usuário 7
INSERT INTO tutoria."USUARIO_TEMA" (nivel_conhecimento, fk_usuario_id, fk_tema_id)
VALUES (4, 7, 1), (3, 7, 2), (2, 7, 3), (1, 7, 4), (4, 7, 5);

-- Usuário 8
INSERT INTO tutoria."USUARIO_TEMA" (nivel_conhecimento, fk_usuario_id, fk_tema_id)
VALUES (2, 8, 1), (3, 8, 2), (1, 8, 3), (4, 8, 4), (2, 8, 5);

-- Usuário 9
INSERT INTO tutoria."USUARIO_TEMA" (nivel_conhecimento, fk_usuario_id, fk_tema_id)
VALUES (3, 9, 1), (2, 9, 2), (1, 9, 3), (4, 9, 4), (3, 9, 5);

-- Usuário 10
INSERT INTO tutoria."USUARIO_TEMA" (nivel_conhecimento, fk_usuario_id, fk_tema_id)
VALUES (1, 10, 1), (4, 10, 2), (2, 10, 3), (3, 10, 4), (1, 10, 5);

#INSERT DE FUNCIONÁRIOS

INSERT INTO tutoria."FUNCIONARIO" (salario, fk_usuario_id, matricula)
VALUES (5000.00, 1, 'MAT12345');

INSERT INTO tutoria."FUNCIONARIO" (salario, fk_usuario_id, matricula)
VALUES (6000.00, 2, 'MAT67890');

#INSERT DE TEMAS

INSERT INTO tutoria."TEMA" (fk_categoria_id, descricao)
VALUES (1, 'Álgebra Linear');

INSERT INTO tutoria."TEMA" (fk_categoria_id, descricao)
VALUES (1, 'Cálculo Diferencial');

INSERT INTO tutoria."TEMA" (fk_categoria_id, descricao)
VALUES (2, 'Biologia Celular');

INSERT INTO tutoria."TEMA" (fk_categoria_id, descricao)
VALUES (2, 'Química Orgânica');

INSERT INTO tutoria."TEMA" (fk_categoria_id, descricao)
VALUES (3, 'Idade Média');

INSERT INTO tutoria."TEMA" (fk_categoria_id, descricao)
VALUES (3, 'Segunda Guerra Mundial');

INSERT INTO tutoria."TEMA" (fk_categoria_id, descricao)
VALUES (4, 'Pintura a Óleo');

INSERT INTO tutoria."TEMA" (fk_categoria_id, descricao)
VALUES (4, 'Escultura em Argila');

INSERT INTO tutoria."TEMA" (fk_categoria_id, descricao)
VALUES (5, 'Inglês Avançado');

INSERT INTO tutoria."TEMA" (fk_categoria_id, descricao)
VALUES (5, 'Espanhol Básico');

#INSERT DE CATEGORIA

INSERT INTO categorias (descricao)
VALUES
    ('Matemática'),
    ('Ciências'),
    ('História'),
    ('Artes'),
    ('Idiomas'),
    ('Programação'),
    ('Música'),
    ('Esportes'),
    ('Saúde'),
    ('Negócios');

```

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
