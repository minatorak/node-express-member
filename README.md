# RESTful API with Node Express Example

## installation & start

# install docker for mac os

check docker version

# start docker
docker-compose up --build -d

npm install

npm run mon

## simple connect api with postman
method: post
http://localhost:3000/users
Body: raw -> json

```
{
	"login": "minatorak",
	"password": "password1234"
}
```


## Create User

**Method:** POST
**Endpoint:** /users

```
{
	"login": "john",
	"password": "password"
}
```

## Authenticate User

**Method:** POST
**Endpoint:** /auth/login

```
{
	"login": "john",
	"password": "password"
}
```

## Update user profile

**Method:** POST
**Endpoint:** /users/:id
**Remark:** This API requires access token returned from login API as Auth Bearer

```
{
	"display": "John Farmer"
}
```
