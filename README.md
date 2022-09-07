

# Fluxos  API

<img align='right' src='./assets/logo.svg' width=200px >

Estou criando um Sistema de fluxo de caixa para mim, controlar minha finanças e abandonar as tabelas de excel


### Indice 💰

1. Introdução
2. Requisitos e Desenvolvimento
3. Como Instalar
4. Como Usar
5. Considerações Finais
6. Licença

## Introdução 💵


Uma esse desenlvovimento foi um projeto do Curso ProgramadorBr, sendo que a estilização dos dos elementos teve um toque especial das minhas mãos.

## Requisitos e Desenvolvimento 🤳🔧


**Desenvolvimento** 



<img width=80 src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original-wordmark.svg" />

<img  width=80 src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/express/express-original-wordmark.svg" />

<img width=90 src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original-wordmark.svg" />

          



**Requisitos**

*Usuário*

Criar usuário com login e suas Operações de CRUD.

Manter usuário com controle de acesso selecionando o permissões de prévilegios.

*Fluxo de caixa*

Possível realizar as operações básica de CRUD e nós mesmo e possível selecionar classificações de dados personalizadas conforme critério que administrador queira. Você verá posteriormente:

*Classificações*

Será possível também criar como foi dito acima, tipos de classificações personalizadas. Todas eles serão atrelados ao id item do fluxo de caixa:

Exemplo: Classificação Elementos

```markdown
[
	{
		"idelementos": 1,
		"descricao_elementos": ""
	},
	{
		"idelementos": 5,
		"descricao_elementos": "Ativo"
	}
]
```

Exemplo: Fluxo de caixa:

```markdown
[
	{
		"id_item_fluxo": 1,
		"dia_item_fluxo": 16,
		"mes_item_fluxo": 7,
		"ano_item_fluxo": 2022,
		"hora_item_fluxo": "12:40:59",
		"descricao_elementos": "",
		"descricao_subelementos": "",
		"descricao_tipos": "",
		"descricao_subtipos": "",
		"descricao_minitipos": "",
		"descricao_nanotipos": "",
		"descricao_item_fluxo": "Saldo Anterior",
		"valor_item_fluxo": "0.00",
		"saldo_atual": "0.00"
	},
	{
		"id_item_fluxo": 2,
		"dia_item_fluxo": 22,
		"mes_item_fluxo": 7,
		"ano_item_fluxo": 2022,
		"hora_item_fluxo": "18:31:27",
		"descricao_elementos": "",
		"descricao_subelementos": "",
		"descricao_tipos": "",
		"descricao_subtipos": "",
		"descricao_minitipos": "",
		"descricao_nanotipos": "",
		"descricao_item_fluxo": "Ganhei na loteria",
		"valor_item_fluxo": "100.00",
		"saldo_atual": "100.00"
	},
```

## Como Instalar 🪛

**Usarem o Mysql workbeanch em nosso tutorial**

1.Tenha um **NODEjs** e **Mysql 8.0** instalado.

2. Clone o projeto.

3. Importe o dump do banco de dados. Localizado no caminho abaixo:


        Model\dblfluxosnodb20220902.sql



<img  align='left' src="./assets/dbimport.png">


4. Nomeie um Schema da importação conforme o seu critério com a imagem:

<img  align=center src="./assets/dbconfigs.png">


4. Entre no Diretorio no **CMD ou em Outro terminal** de comando.

5. Em seguida volte na pasta raiz


6. **ATENÇÃO** Após isso digite o npm install se caso o dotenv nao for instalado dentro da pasta **raiz** do projeto.

7. Após isso crie um **.env** na pasta **raiz** e configure apontando para sua base de dados. Conforme abaixo ou como sua preferencia :

Exemplo nao preenchido no arquivo .env.example:

                PORT_SERVIDOR=

                USERDB=
                PORTDB=
                HOSTDB=
                DATABASE=
                PASSWORD=

                TOKEN_SECRET=


Exemplo preenchido  .env:


                PORT_SERVIDOR=3000

                USERDB="root"
                PORTDB=3306
                HOSTDB="127.0.0.1"
                DATABASE="db_controllerfluxo"
                PASSWORD="admin"

                TOKEN_SECRET="joao"



8.Após volte para pasta **raiz** e digite seguinte comando abaixo:

        npm start



5. TCHAM RAMMM Rodando !
6. Use uma API de teste do seu agrado. Ex:Postman, ou Insommia.
7. Importe o arquivo HAR. Path: /api/api-fluxos-v1-har

## Como usar 👨‍💻

**Iniciar:**

### Clique aqui para acessar a documentação completa da API..
<a href='https://docs-fluxosapi.netlify.app' >Clique aqui</a>

1. Faça login rota inicial. Exemplo: http://localhost:3000/login
2. Busque o token de acesso na chave do Json Resposta : “tokenUser”
3. Coloque no cabeçalho
4. E siga as rotas.
5. Rota principal fluxo de caixa pode cadastrar um item e classificá-lo conforme o id a aplicação.

**Classificações:**

Poderá Inserir, deletar, criar, editar qualquer uma dessas. Igual na API:

- Elementos
- Subelementos
- Tipos
- Subtipos
- Minitipos
- Nanotipos

## Considerações Finais ✍️

Bom... Isso é somente a API da aplicação. O Front será desenvolvido em outra breve..
Valeu por passar aqui! 😉Um abração de Ursoo 🐻! Volte sempre!

## Autor

Feito com 🤭 por Joao Guilherme 👋🏽 Entre em contato!

[![Linkedin Badge](https://img.shields.io/badge/-Joao-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/jaoo/)](https://www.linkedin.com/in/joaog123/) 
[![Badge](https://img.shields.io/badge/-joaoguilherme94@live.com-c80?style=flat-square&logo=Microsoft&logoColor=white&link=mailto:joaoguilherme94@live.com)](mailto:joaoguilherme94@live.com)

### **License**
[![Licence](https://img.shields.io/github/license/Ileriayo/markdown-badges?style=for-the-badge)](./LICENSE)