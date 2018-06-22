# Update Product by ID

Update the Product call this method.

**URL** : `/api/v1/{seller}/product/{id}`

**Method** : `PUT`

**Auth required** : YES

**Permissions required** : None

**Data constraints**

```json
{
    "name": "[unicode 64 chars max]"
}
```

**Data example** Partial data is allowed, but there is only one field.

```json
{
    "name": "Build something project dot com",
}
```

## Success Responses

**Condition** : Update can be performed either fully or partially by the Owner
of the Account.

**Code** : `200 OK`

**Content example** : For the example above, when the 'name' is updated and
posted to `/api/accounts/123/`...

```json
{
    "id": 123,
    "name": "New project name",
    "enterprise": false,
    "url": "http://testserver/api/accounts/123/"
}
```

## Error Response

**Condition** : Account does not exist at URL

**Code** : `404 NOT FOUND`

**Content** : `{}`

## Notes

### Data ignored

Endpoint will ignore irrelevant and read-only data such as parameters that
don't exist, or `id` and `enterprise` fields which are not editable.

E.g. if Account already exits:

**Data example**

```json
{
    "wibble": "flobble",
    "id": 987,
    "enterprise": true
}
```

**Code** : `200 OK`

**Content example**

```json
{
    "id": 123,
    "name": "New project name",
    "enterprise": false,
    "url": "http://testserver/api/accounts/123/"
}
```
