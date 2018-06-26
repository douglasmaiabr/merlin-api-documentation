# Show Order by ID

Get the details of the currently Authenticated User along with basic
subscription information.

**URL** : `/api/v1/{seller}/order/1`

**Method** : `GET`

**Auth required** : YES

**Permissions required** : None

## Success Response

**Code** : `200 OK`

**Content examples**

For a Order with ID 1 on the database.

```json
[  
   {  
      "id":1,
      "magento_increment_id":"100000045",
      "company":"CAMAFEU GOURMET CAFETERIA LTDA",
      "company_name":"CAMAFEU",
      "cnpj":"14784634000197\t",
      "ie":"201928233",
      "address_street":"AV POMPEIA",
      "address_number":"123",
      "address_complement":"",
      "address_zone":"BARRA FUNDA",
      "address_city":"SAO PAULO",
      "address_state":"SP",
      "address_postcode":"03452000",
      "address_country":"BR",
      "telephone":"1143440909",
      "mobile":"11989002324",
      "email":"contato@camafeu.com",
      "contact":"PAULO",
      "salesman":"ALINE",
      "shipping_period":"TARDE",
      "protest":"0",
      "score":"890",
      "website":"MENUPONTOCOM",
      "product_id":"3008",
      "name":"DP REXONA 100G EFFICENT",
      "sku_magento":"ROG3128",
      "sku_seller":"3128",
      "qtd":2,
      "price":10,
      "discount":0,
      "total":20,
      "status":1,
      "created_at":"2018-06-26 00:00:00"
   },
   {  
      "id":2,
      "magento_increment_id":"100000045",
      "company":"CAMAFEU GOURMET CAFETERIA LTDA",
      "company_name":"CAMAFEU",
      "cnpj":"14784634000197\t",
      "ie":"201928233",
      "address_street":"AV POMPEIA",
      "address_number":"123",
      "address_complement":"",
      "address_zone":"BARRA FUNDA",
      "address_city":"SAO PAULO",
      "address_state":"SP",
      "address_postcode":"03452000",
      "address_country":"BR",
      "telephone":"1143440909",
      "mobile":"11989002324",
      "email":"contato@camafeu.com",
      "contact":"PAULO",
      "salesman":"ALINE",
      "shipping_period":"TARDE",
      "protest":"0",
      "score":"890",
      "website":"MENUPONTOCOM",
      "product_id":"3009",
      "name":"CR TRIM TRAT 65G CABELO",
      "sku_magento":"ROG3487",
      "sku_seller":"3487",
      "qtd":2,
      "price":10,
      "discount":0,
      "total":20,
      "status":1,
      "created_at":"2018-06-26 00:00:00"
   }
]
```

