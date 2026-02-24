Rotating proxy resellers must first read the 👉 [**Access Pre-Instruction Document**](https://www.ipfoxy.com/help/docs/jie-ru-qian-zhi-shuo-ming-wen-dang-bi-kan) and complete the **API access application and registration** process.
Once approved, you will be able to allocate traffic to accounts via the following API:

**Path:** /ip/open-api/allocate-flow-sub-account

**Method:** POST

Parameter Description:

| Parameter name  | Is it necessary | Example       | Remark                                                       |
| --------------- | --------------- | ------------- | ------------------------------------------------------------ |
| account         | yes             | ABCDEFHGJ2000 | account                                                      |
| flow            | yes             | 1024          | Traffic MB 1024                                              |
| idempotency_key | yes             | ABCDEFHGJ2000 | All operations unique identifier length 10-25                |
| day             | no              | 0             | The traffic expiration time can be: 0 (indefinite), 30, 90, 180, 360 (unit: day), the default value is 0 |

**Interface description: Rotating proxy reseller allocate traffic to accounts**

**Return data:**

```javascript
 {
    "data": {},
    "code": 0,
    "msg": "Success"
}
```