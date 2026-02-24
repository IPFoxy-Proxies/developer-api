# Automatic Renewal

**Path:** /ip/open-api/auto-extend

**Method:** POST

**Interface description: Enable/disable automatic renewal**

Parameter description:

| Parameter name | Is it necessary? | Example | Remark                                        | Use cases |
| -------------- | ---------------- | ------- | --------------------------------------------- | --------- |
| auto_extend | yes              | 1       | 1 on 0 off                                    |           |
| proxy_ids      | yes              | i14iudm | Proxy IDs, multiple ones separated by commas. |           |

**Note:** Batch operations are limited to a maximum of **300 proxies** at a time. Separate notifications will be sent if individual proxies expire or are shared. In multi-proxy operations involving expired or shared proxies, the system will only process **valid, exclusive proxies**.

**Returned data:**

```javascript
 {
    "data": {},
    "code": 0,
    "msg": "Success"
}

```
