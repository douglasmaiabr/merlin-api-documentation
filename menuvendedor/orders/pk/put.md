# Update Product by ID

Allow the Authenticated User to update their details.

**URL** : `/api/v1/{sellers}/order/{id}`

**Method** : `PUT`

**Auth required** : YES

**Permissions required** : None

**Data constraints**

```json
{
    "status":"[string]",
    "qty":"[decimal]",
    "price": "[decimal]"
}
```

**Data examples**

Partial data is allowed.

```json
{
    "status":"faturado",
    "qty":25.00,
    "price": 10.95 
}
```

## Success Responses

**Condition** : Data provided is valid and User is Authenticated.

**Code** : `204 Updated`

## Error Response

**Condition** : If provided data is invalid, e.g. a name field is too long.

**Code** : `400 BAD REQUEST`
