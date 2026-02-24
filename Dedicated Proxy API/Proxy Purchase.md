# Proxy Purchase

**Path:** /ip/open-api/proxy-buy

**Method:** POST

**Interface description: Purchase proxy**

Parameter description:

| Parameter name | Is it necessary | Example | Remarks                                    | Usage scenarios |
| -------------- | --------------- | ------- | ------------------------------------------ | --------------- |
| days           | Yes             | 30      | Number of days (supports 30, 90, 180, 360) |                 |
| area_id        | Yes             | 239     | Region ID                                  |                 |
| auto_extend    | Yes             | 1       | Auto-renewal 0 off 1 on                    |                 |
| num            | Yes             | 1       | Quantity <= 100                            |                 |

 

**Return data:**

```javascript
{
  "data": {
    "order_id": "g1k29a2"
  },
  "code": 0,
  "msg": "Success"
}
```

 

Field description:

| order_id | Order ID |
| -------- | -------- |
|          |          |