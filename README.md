# Docker compose

## Execução do projeto

A execução do projeto é feita usando o comando:
```shell
$ docker-compose up
```

Este modelo do Docker Compose fornece um contêiner de BackEnd e FrontEnd do projeto CMPaaS já pré configuradas banco de dados Mongod,
os containers serão executado e o sistema pode ser acessado via http://localhost/ e a api REST em http://localhost:3000/docs.


## Imagens

### mongo
Banco de dados usado para salvar os dados do usuário e mapas

### mongo-express
Visualizador do banco de dados basta acessar http://localhost:8081, é opcional e usado em desenvolvimento

### cmpaas-backend
Api REST para salvar os dados do usuário e mapas conceituais.

Para acessar a documentação com as rotas da api assece: http://localhost:3000/docs 

As variaveis `EMAIL` e `PASSWORD` são configuradas no sistema com um e-mail do projeto, usado para enviar e-mail de recuperação de senha e confirmação de e-mail.

### cmpaas-frontend
Front End feito em AngularJS.
o Front End é exposto na porta 80, porém pode-se editar o arquivo `docker-compose.yml` caso tenha algum conflito de porta.
