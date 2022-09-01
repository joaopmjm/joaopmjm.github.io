## Funcionalidades

No site em si serve apenas para visualizacao dos quizes, e com algumas funcionalidades em relacao ao login, como *logout* ou trocar a senha.

As funcionalidades em relacao aos quizes (add, update, remove) sao via requisicoes a uma API, pode-se fazer isso via software **postman**, a seguir sao as requisicoes possiveis e suas chamadas.

|tipo|caminho|funcionalidade|
|---|---|---|
|POST|{BaseAddress}/?ID={ID do challenge}|Entrega do desafio, fazendo cheques de hora da entrega, se o desafio existe, e promove logica com os dados dentro do QUIZ (Diagnostico, Problema, Codigo, etc...).
