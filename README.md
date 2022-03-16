## Endpoints


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

### retornar todos os pets 

GET /pets

### registar pet

POST /pets

o usuário precisa estar autenticado para realizar o cadastro

registro do pet precisa ir com id do dono

``` 
{
	"name" : "Rex",
	"userId: 2
}
```

### retornar todos os dados de um user e seus pets

GET /users/{userId}?_embed=pets

### editar info de algum pet

o usuário precisa estar autenticado para realizar as alterações do pet

PUT /pets/{petId}

o corpo da requisição precisa ir com a referência do id do dono

```
{
	"name" : "Rex",
	"userId" : 4
}
```
### deletar pet 

o usuário precisa estar autenticado para deletar os pets

DELETE /pets/{petId}


