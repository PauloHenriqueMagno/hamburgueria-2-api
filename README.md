# json-server-base

Esse é o repositório com a base de JSON-Server + JSON-Server-Auth já configurada, feita para ser usada no desenvolvimento das API's nos Capstones do Q2.

## Endpoints

Assim como a documentação do JSON-Server-Auth traz (https://www.npmjs.com/package/json-server-auth), existem 3 endpoints que podem ser utilizados para cadastro, 2 endpoints que podem ser usados para login, 1 endpoint para editar dados do usuario, 1 endpoint para deletar a conta do usuario e 1 endpoint para visualizar a conta do usuario.

### Cadastro

POST /register <br/>
POST /signup <br/>
POST /users

Qualquer um desses 3 endpoints irá cadastrar o usuário na lista de "Users", sendo que os campos obrigatórios são os de email e password.
Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.

### Login

POST /login <br/>
POST /signin

Qualquer um desses 2 endpoints pode ser usado para realizar login com um dos usuários cadastrados na lista de "Users"

### Editar

PUT /users/id

Utilizando essa endpoint ira modificar qualquer dado do usuario e criar qualquer nova propriedade sendo obrigatório o token da conta

### Deletar

DELETE /users/id

Essa endpoint ira deleta sua conta sendo obrigatório o token da conta

### Visualizar

PATCH /users/id

Essa endpoint ira mostra os dados da sua conta sendo obrigatório o token da conta