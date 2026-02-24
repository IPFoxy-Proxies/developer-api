# Proxy Renewal

**Path:** /ip/open-api/proxy-buy

**Method:** POST

**Interface description: Purchase proxy**

Parameter description:

| Parameter name | Is it required | Example | Remarks                                | Usage scenarios |
| -------------- | -------------- | ------- | -------------------------------------- | --------------- |
| days           | Yes            | 30      | Number of days                         |                 |
| proxy_ids      | Yes            | i14iudm | Proxy ID, multiple separated by commas |                 |

**Note: The number of proxies renewed each time cannot exceed 300.**

**Return data:**

```javascript
{
  "data": {
    "order_id": "g1k3bk5"
  },
  "code": 0,
  "msg": "Success"
}
```

 

Field description:

| order_id | Order ID |
| -------- | -------- |
|          |          |