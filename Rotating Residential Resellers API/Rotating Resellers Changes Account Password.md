# Rotating Resellers Changes Account Password

Rotating proxy resellers must first read the 👉 [**Access Pre-Instruction Document**](https://www.ipfoxy.com/help/docs/jie-ru-qian-zhi-shuo-ming-wen-dang-bi-kan) and complete the **API access application and registration** process.
Once approved, you will be able to changes account password via the following API:

**Path:** /ip/open-api/update-pass

**Method:** POST

Parameter Description:

| Parameter name | Is it necessary | Example       | Remark                |
| -------------- | --------------- | ------------- | --------------------- |
| account        | yes             | ABCDEFHGJ2000 | Account               |
| password       | yes             | ABCDEFGHI2000 | Password length 10-15 |

**Interface description: Rotating proxies changes account and password**

**Return data:**

```javascript
 {
    "data": {},
    "code": 0,
    "msg": "Success"
}
```