# Merlin API Documentation

These examples were taken from projects mainly using [Django Rest
Framework](https://github.com/tomchristie/django-rest-framework) and so the
JSON responses are often similar to the way in which DRF makes responses.

Where full URLs are provided in responses they will be rendered as if service
is running on 'https://merlin.com.vc/'.

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
* [Show info](products/get.md) : `GET /api/v1/{seller}/product/{id}`
* [Update info](products/put.md) : `PUT /api/v1/{seller}/product/{id}`

### Orders

Endpoints for viewing and manipulating the Orders that the Authenticated User
has permissions to access.

* [List all](accounts/get.md) : `GET /api/v1/{seller}/orders`
* [Show info](accounts/pk/get.md) : `GET /api/v1/{seller}/order/{id}`
* [Update info](accounts/pk/put.md) : `PUT /api/v1/{seller}/order/{id}`
