# Rotating Resellers Account Creation

Rotating proxy resellers must first read the 👉 [**Access Pre-Instruction Document**](https://www.ipfoxy.com/help/docs/jie-ru-qian-zhi-shuo-ming-wen-dang-bi-kan) and complete the **API access application and registration** process.
Once approved, you will be able to create account via the following API:

**Path:** /ip/open-api/create-sub-account

**Method:** POST

Parameter Description:

| Parameter name  | Is it necessary | Example       | Remark                                                       |
| --------------- | --------------- | ------------- | ------------------------------------------------------------ |
| account         | yes             | ABCDEFHGJ2000 | Account length 10-15                                         |
| password        | yes             | ABCDEFHGJ2000 | Password length 10-15                                        |
| flow            | yes             | 1024          | Traffic MB                                                   |
| idempotency_key | yes             | ABCDEFHGJ2000 | All operations unique identifier length 10-25                |
| day             | no              | 0             | The traffic expiration time can be: 0 (indefinite), 30, 90, 180, 360 (unit: day), the default value is 0 |

**Interface description: Rotating proxies account creation**

**Return data:**

```javascript
 {
    "data": {
        "account": "ABCDEFHGJ2000",
        "password": "ABCDEFHGJ2000"
    },
    "code": 0,
    "msg": "Success"
}
```

Field Description:

| account  | account  |
| -------- | -------- |
| password | password |