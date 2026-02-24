Rotating proxy resellers must first read the 👉 [**Access Pre-Instruction Document**](https://www.ipfoxy.com/help/docs/jie-ru-qian-zhi-shuo-ming-wen-dang-bi-kan) and complete the **API access application and registration** process.
Once approved, you will be able to changes account whitelist via the following API:

**Path:** /ip/open-api/update-ip-whitelist

**Method:** POST

Parameter Description:

| Parameter name | Is it necessary | Example         | Remark                                                       |
| -------------- | --------------- | --------------- | ------------------------------------------------------------ |
| account        | yes             | ABCDEFHGJ2000   | account                                                      |
| ip             | yes             | 1.1.1.1,2.2.2.2 | Whitelist: supports multiple IPs, separated by commasCancel whitelist: pass an empty string "" to clear all whitelists |

**Interface description: Rotating proxy reseller changes account whitelist**

**Return data:**

```javascript
 {
    "data": {},
    "code": 0,
    "msg": "Success"
}
```