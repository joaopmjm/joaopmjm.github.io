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