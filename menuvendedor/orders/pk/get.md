# Show product by ID

Get the details of the currently Authenticated User along with basic
subscription information.

**URL** : `/api/v1/{seller}/products/`

**Method** : `GET`

**Auth required** : YES

**Permissions required** : None

## Success Response

**Code** : `200 OK`

**Content examples**

For a Product with ID 2216 on the local database where that Product has saved an
email address and name information.

```json
{  
   "id":2116,
   "name":"BANDEIJA PARA ESFIHA 23CM PCT 25UN",
   "seller_sku":"0900",
   "magento_sku":"MCA0900",
   "magento_id":2121,
   "magento_url":"bandeija-para-esfiha-23cm-pct-25un",
   "images":null,
   "ean":"7896713100099",
   "dum":null,
   "unity":"PCT",
   "weight":"0.50",
   "lenght":null,
   "height":null,
   "width":null,
   "price":20.59,
   "multiplier":10,
   "forkg":1,
   "status":1,
   "description":"BANDEIJA PARA ESFIHA 23CM PCT 25UN(CAIXA C/ 25 UNIDADES) para comprar online. Quer saber se é seguro comprar na Menu? Este produto é vendido e entregue por: Monte Carlo Alimentos, distribuidor com anos de experiencia.",
   "short_description":"BANDEIJA PARA ESFIHA 23CM PCT 25UN(CAIXA C/ 25 UNIDADES) / Produto vendido e entregue por: Monte Carlo Alimentos em Entregue em até 48h",
   "brand":"JUNE",
   "qty":50,
   "seller":"montecarlo",
   "categories": [
        2, 102, 144
   ],
   "crossdocking_days": 1,
   "created_at":"2018-01-17 02:25:40",
   "updated_at":"2018-01-21 10:29:53",
   "deleted_at": null
}
```

For a user with ID 4321 on the local database but no details have been set yet.

```json
{
    "id":1537,
    "name":null,
    "seller_sku":"1322",
    "magento_sku":"MCA1322",    
    "magento_id":2365,
    "magento_url":"azeitona-verde-calib-24-28-bd-15kg",
    "images":null,
    "ean":null,
    "dum":null,
    "unity":null,
    "weight":null,
    "lenght":null,
    "height":null,
    "width":null,
    "price":null,
    "multiplier":null,
    "forkg":null,
    "status":null,
    "description":null,
    "short_description":null,
    "brand":null,
    "qty":null,
    "seller":"montecarlo",
    "categories":null,
    "crossdocking_days":null,
    "created_at":"2018-01-17 02:25:39",
    "updated_at":"2018-01-21 10:29:52",
    "deleted_at":null
}
```

## Notes

* If the User does not have a `UserInfo` instance when requested then one will
  be created for them.
