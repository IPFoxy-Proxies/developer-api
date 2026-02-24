# Get order information

**Path:** /ip/open-api/order-info

**Method:** GET

**Interface description: Query purchased proxies**

Parameter description:

| Parameter name | Is it Required | Example | Remarks  | Usage scenarios |
| -------------- | -------------- | ------- | -------- | --------------- |
| order_id       | Yes            | g1k29a2 | Order ID |                 |

 

**Return data:**

```javascript
{
  "data": {
    "id": "g1k29a2",
    "total_price": "17.97",
    "proxy_ids": [
      "i14iudm",
      "i14iuqn",
      "i14iv4o"
    ],
    "proxy_count": "3",
    "order_type": "BUY"
  },
  "code": 0,
  "msg": "Success"
}
```

 

Field description:

| id          | Order ID                                     |
| ----------- | -------------------------------------------- |
| total_price | Order amount (actual deduction)              |
| proxy_ids   | Proxy ID collection                          |
| proxy_count | Number of proxies purchased/renewed in order |
| order_type  | Order type BUY new purchase  EXTEND renewal  |