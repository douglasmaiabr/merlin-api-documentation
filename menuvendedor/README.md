# Menu Vendedor API Documentation

Where full URLs are provided in responses they will be rendered as if service
is running on 'https://menuvendedor.com/'.

## Open Endpoints

Open endpoints require no Authentication.

* [Login](login.md) : `POST /api/v1/login/`

## Endpoints that require Authentication

Closed endpoints require a valid Token to be included in the header of the
request. A Token can be acquired from the Login view above.

### Products

Endpoints for viewing and manipulating the Products that the Authenticated User
has permissions to access.

* [List all](products/get.md) : `GET /api/v1/{seller}/products`
* [Show info](products/pk/get.md) : `GET /api/v1/{seller}/product/{id}`
* [Update info](products/pk/put.md) : `PUT /api/v1/{seller}/product/{id}`

### Orders

Endpoints for viewing and manipulating the Orders that the Authenticated User
has permissions to access.

* [List all](accounts/get.md) : `GET /api/v1/{seller}/orders`
* [Show info](accounts/pk/get.md) : `GET /api/v1/{seller}/order/{id}`
* [Update info](accounts/pk/put.md) : `PUT /api/v1/{seller}/order/{id}`
