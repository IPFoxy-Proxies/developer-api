# Rotating Resellers Obtains Account Traffic Information

Rotating proxy resellers must first read the 👉 [**Access Pre-Instruction Document**](https://www.ipfoxy.com/help/docs/jie-ru-qian-zhi-shuo-ming-wen-dang-bi-kan) and complete the **API access application and registration** process.
Once approved, you will be able to retrieve account traffic information via the following API:

**Path:** /ip/open-api/get-sub-account-flow

**Method:** GET

Parameter Description:

| Parameter name | Is it necessary | Example       | Remark                                |
| -------------- | --------------- | ------------- | ------------------------------------- |
| account        | yes             | ABCDEFHGJ2000 | Account created through the interface |

**Interface description: Rotating proxy reseller obtains account traffic (one-minute cache)**

**Return data:**

```javascript
 {
    "data": {
        "surplus_flow": "5242880",
        "use_flow": "0",
        "unit": "KB"
    },
    "code": 0,
    "msg": "Success"
}
```

Field Description:

| surplus_flow | Remaining flow |
| ------------ | -------------- |
| use_flow     | Use data       |
| unit         | Unit: KB       |