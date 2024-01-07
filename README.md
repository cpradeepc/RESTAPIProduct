
# REST API OF PRODUCT ONLINE APPLICATION

This is a Product items Web API with hash and jwt token security.
when any user want to access the data and do CRUD operation , firstly he need of signup and signin.
when the user will have  signin into API, the will be generated the token for given time accessable( here gave 2 minute expire time of authentication).
user is able to access the API otherwise showing the message unauthorized user .

# REST API

The REST API to the example app is described below.

### Request
Prefix with /api/...
`GET /product/`

    curl -i -H 'Accept: application/json' http://localhost:8055/api/product

## Create a account

### Request

`POST /signup/`

    curl -i -H 'Accept: application/json' -d 'credential{...}' localhost:8055/api/signup


## login account

### Request

`POST /signin/`

    curl -i -H 'Accept: application/json' -d 'credential{...}' localhost:8055/api/signin
## Create a new Product items

### Request

`POST /product/`

    curl -i -H 'Accept: application/json' -d 'product{...}' localhost:8055/api/product


## Get a  Product item

### Request

`GET /product`

    curl -i -H 'Accept: application/json' localhost:8055/api/product

## Get a specific Product item

### Request

`GET /product/id`

    curl -i -H 'Accept: application/json' localhost:8055/api/product/1

## Update a specific Product item

### Request

`PUT /product/id`

    curl -i -H 'Accept: application/json' -d 'product{...}' localhost:8055/api/product/1


## Delete a specific Product item

### Request

`DELETE /product/id`

    curl -i -H 'Accept: application/json' localhost:8055/api/product/1
