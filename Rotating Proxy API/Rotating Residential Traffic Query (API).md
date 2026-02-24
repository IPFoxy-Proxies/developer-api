# Rotating Residential Traffic Query (API)

**Rotating residential traffic flow can be queried via the following API:**

**Path:** /ip/open-api/residential-data

**Method:** GET

Parameter description:

| Parameter name | Is it necessary? | Example | Remark                                                       | Use cases                      |
| -------------- | ---------------- | ------- | ------------------------------------------------------------ | ------------------------------ |
| account        | no               | ABC2000 | The authentication account in the proxy account information customer-ABC2000 | Default query for main account |

**Interface Description: Retrieves rotating residential traffic information.**

**Returned data:**

```javascript
 {
    "data": {
        "query_time": "1724055635",
        "expire_time": "1726644469",
        "total_mb": "644981.47",
        "remain_mb": "431955.06"
    },
    "code": 0,
    "msg": "Success"
}
```

Field description:

| query_time  | Query timestamp                |
| ----------- | ------------------------------ |
| expire_time | Package expiration time stamp  |
| remain_mb   | Remaining data allowance in MB |
| total_mb    | Total package size (in MB)     |