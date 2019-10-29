# Docker compose

## Execução
Para execução do projeto é necessário docker e docker compose-instalado, que podem ser adiquiridos [neste site](https://get.docker.com/) para usuarios linux ou [neste](https://www.docker.com/) para usuarios Windows.

Após a instalação, a execução do projeto é feita usando o comando `docker-compose up` dentro da pasta do projeto, as imagens serão montadas e executadas em ordem.


## Imagens

### mongo
Banco de dados usado para salvar os dados do usuário e mapas

### mongo-express
Visualizador do banco de dados basta acessar http://localhost:8081, é opcional e usado em desenvolvimento

### cmpaas-backend
Api REST para salvar os dados do usuário e mapas conceituais.
As variaveis `EMAIL` e `PASSWORD` são configuradas no sistema com um e-mail do projeto, usado para enviar e-mail de recuperação de senha e confirmação de e-mail.

### cmpaas-frontend
Front End feito em Angularjs 
