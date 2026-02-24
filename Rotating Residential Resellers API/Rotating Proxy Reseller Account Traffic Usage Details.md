Rotating proxy resellers must first read the 👉 [**Access Pre-Instruction Document**](https://www.ipfoxy.com/help/docs/jie-ru-qian-zhi-shuo-ming-wen-dang-bi-kan) and complete the **API access application and registration** process.
Once approved, you will be able to obtain account traffic usage details via the following API:

**Path:** /ip/open-api/get-account-use-flow-list

**Method:** GET

Parameter Description:

| Parameter name  | Is it necessary | Example       | Remark                                                       |
| --------------- | --------------- | ------------- | ------------------------------------------------------------ |
| account         | yes             | ABCDEFHGJ2000 | account                                                      |
| start_time      | yes             | 1725206401    | Start timestamp, minimum value is 90 days ago                |
| end_time        | yes             | 1725292799    | End timestamp                                                |
| unit            | yes             | 2             | 1 hour dimension 2 day dimension                             |
| page            | no              | 1             | Page number: Default 1                                       |
| page_size       | no              | 20            | Pages: Default is 20, and the number of pages displayed per page is between 10 and 100 |
| timezone_offset | no              | 0             | The default value is 0, which divides the time span into UTC+8. |

**Interface description: Rotating proxy reseller account traffic usage details**

**Return data:**

```javascript
 {
    "data": {
        "list": [
            {
                "date": "2025-06-26 00:00:00",
                "account": "ABCDEFHGJ2000",
                "flow": "11"
            },
            {
                "date": "2025-06-25 00:00:00",
                "account": "ABCDEFHGJ2000",
                "flow": "22"
            },
            {
                "date": "2025-06-24 00:00:00",
                "account": "ABCDEFHGJ2000",
                "flow": "33"
            }
        ],
        "unit": "MB",
        "count": "8",
        "timezone": "+08:00"
    },
    "code": 0,
    "msg": "Success"
}
```

Field Description:

| date    | date           |
| ------- | -------------- |
| account | account        |
| flow    | Use traffic MB |
| count   | quantity       |