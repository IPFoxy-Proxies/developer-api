# Get order price

**Path:** /ip/open-api/order-price

**Method:** GET

**Interface description: used to obtain the order price of purchasing/renewing** **proxies**

Parameter description:

| Parameter name | Is it required | Example | Remarks                         | Usage scenarios |
| -------------- | -------------- | ------- | ------------------------------- | --------------- |
| order_type     | Yes            | BUY     | EXTEND renewal BUY new purchase |                 |
| days           | Yes            | 30      | Number of days                  |                 |
| area_id        | No             | 239     | Region ID                       | New purchase    |
| proxy_ids      | No             |         | Proxy ID                        | Renewal         |
| num            | No             | 1       | Quantity <= 100                 | New purchase    |

 

**Return data:**

```javascript
{
  "data": {
    "order price": "11.98",
    "order_type": "EXTEND"
  },
  "code": 0,
  "msg": "Success"
}
```

 

Field description:

| id          | Proxy region ID                             |
| ----------- | ------------------------------------------- |
| order price | Price                                       |
| order_type  | Order type: BUY new purchase EXTEND renewal |