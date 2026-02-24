# Rotating Resellers Obtains Account List

Rotating proxy resellers must first read the 👉 [**Access Pre-Instruction Document**](https://www.ipfoxy.com/help/docs/jie-ru-qian-zhi-shuo-ming-wen-dang-bi-kan) and complete the **API access application and registration** process.
Once approved, you will be able to retrieve account list via the following API:

**Path:** /ip/open-api/get-sub-account-list

**Method:** GET

Parameter Description:

| Parameter name | Is it necessary | Example       | Remark                                                       |
| -------------- | --------------- | ------------- | ------------------------------------------------------------ |
| account        | no              | ABCDEFHGJ2000 | Get the list of accounts created through the interface       |
| page           | no              | 1             | Page number: Default 1                                       |
| page_size      | no              | 20            | Pages: Default is 20, and the number of pages displayed per page is between 10 and 100 |

**Interface description: Rotating proxies obtains account list**

**Return data:**

```javascript
 {
    "data": {
        "list": [
            {
                "account": "yDMKIRX5aC",
                "password": "askdjhaskdjaslkjdaskldj",
                "status": "1",
                "surplus_flow": "52428800",
                "use_flow": "0",
                "ip_whitelist": "1.1.1.1,2.2.2.2",
                "created_time": "1747904273",
                "ex_time": "2147483647",
                "unit": "KB",
                "is_main": "1",
            },
            {
                "account": "eHhQVbaj",
                "password": "U2QGKxfG",
                "status": "1",
                "surplus_flow": "2692215418",
                "use_flow": "1012547520",
                "ip_whitelist": "",
                "created_time": "1687252074",
                "ex_time": "2147483647",
                "unit": "KB",
                "is_main": "2"
            }
        ],
        "total": "2"
    },
    "code": 0,
    "msg": "Success"
}
```

Field Description:

| account      | account                              |
| ------------ | ------------------------------------ |
| password     | password                             |
| status       | Account status: 1 normal; 2 disabled |
| surplus_flow | Remaining flow                       |
| use_flow     | Use data                             |
| ip_whitelist | IP whitelist                         |
| created_time | Creation time (timestamp)            |
| ex_time      | Expiration time (timestamp)          |
| unit         | Unit: KB                             |
| total        | total                                |
| is_main      | 1 Main account 2 Sub accounts        |