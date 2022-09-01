# open-dev-2022.2-pro-project

### Objetivo: entender como rodar sem instrucoes
# Como rodar
## Dependencias
- SQLite3, *$pip install sqlite3*
- Flask, *$pip install Flask*
- Flask http auth, *$pip install flask_httpauth*
## Pre-run
1. Installar o SQliteBrowser, *$snap install sqlitebrowser*.
1. Rodar o gerenciador de Banco de dados *$sqlitebrowser*.
1. Criar um banco de dados zerado, *file-> New Database*
1. Na aba *Execute SQL* copiar o codigo contido no arquivo *quiz.sql* e colar esse na aba e executar.
1. Na aba *Database Structure* clicar na tabela USER e clicar em *Modify Table*, assim que abrir a aba de modificar, apenas clicar em *OK*
1. Criar um arquivo no root do projeto chamado *user.csv* e adicionar um usuario com a senha, exemplo "*joao,123*", sinceramente pouco importa o segundo valor.
1. Rodar no root *$python adduser.py*, isso vai criar seu usuario
## Run
1. Rodar no root *$python softdes.py*
1. Entrar no Link escrito no terminal em *Running on http://...*
1. Login e senha sao o primeiro valor do CSV criado anteriormente, entao no caso, login *joao* e senha *joao*.

Pronto voce esta dentro.

## Funcionalidades

No site em si serve apenas para visualizacao dos quizes, e com algumas funcionalidades em relacao ao login, como *logout* ou trocar a senha.

As funcionalidades em relacao aos quizes (add, update, remove) sao via requisicoes a uma API, pode-se fazer isso via software **postman**, a seguir sao as requisicoes possiveis e suas chamadas.

|tipo|caminho|funcionalidade|
|---|---|---|
|POST|{BaseAddress}/?ID={ID do challenge}|Entrega do desafio, fazendo cheques de hora da entrega, se o desafio existe, e promove logica com os dados dentro do QUIZ (Diagnostico, Problema, Codigo, etc...).