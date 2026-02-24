# Rotating Residential Traffic History Query (API)

**Historical rotating residential traffic flow can be queried via the following API:**

**Path:** /ip/open-api/residential-data-history

**Method:** GET

**Interface Description: Retrieves rotating residential traffic information.**

Parameter description:

| Parameter name  | Is it necessary? | Example    | Remark                                                       | Use cases                                        |
| --------------- | ---------------- | ---------- | ------------------------------------------------------------ | ------------------------------------------------ |
| is_hour         | no               | 1          | 1 or 0 can be entered; the default is 0.Enter 0 to divide the time span according to UTC+8. | The time interval is 1 for hours and 0 for days. |
| page            | no               | 1          | The value range is [1, 25], with a default of 1; page number |                                                  |
| start_timestamp | yes              | 1725206401 | Start timestamp, minimum value is 90 days ago.               |                                                  |
| end_timestamp   | yes              | 1725292799 | End timestamp                                                |                                                  |
| account         | no               | ABC2000    | The authentication account in the proxy account information customer-ABC2000 | Default query for main account                   |

**Returned data:**

```javascript
 {
    "data": {
        "list": [
            {
                "mb": "1453.16",
                "timestamp": "1725231600",
                "period": "1 hour"
            },
            {
                "mb": "13624.97",
                "timestamp": "1725235200",
                "period": "1 hour"
            },
            {
                "mb": "15726.6",
                "timestamp": "1725238800",
                "period": "1 hour"
            },
            {
                "mb": "10585.6",
                "timestamp": "1725242400",
                "period": "1 hour"
            },
            {
                "mb": "12845.94",
                "timestamp": "1725246000",
                "period": "1 hour"
            },
            {
                "mb": "9128.05",
                "timestamp": "1725249600",
                "period": "1 hour"
            },
            {
                "mb": "6106.33",
                "timestamp": "1725253200",
                "period": "1 hour"
            },
            {
                "mb": "7759.89",
                "timestamp": "1725256800",
                "period": "1 hour"
            },
            {
                "mb": "13815.69",
                "timestamp": "1725260400",
                "period": "1 hour"
            },
            {
                "mb": "9154.83",
                "timestamp": "1725264000",
                "period": "1 hour"
            },
            {
                "mb": "1458.62",
                "timestamp": "1725267600",
                "period": "1 hour"
            }
        ],
        "total": 11,
        "page": 1,
        "page_size": 35
    },
    "code": 0,
    "msg": "Success"
}
```

Field description:

| page_size | Display current page size                                    |
| --------- | ------------------------------------------------------------ |
| page      | Show current page number                                     |
| total     | How many records are there currently?                        |
| list      | Data list                                                    |
| mb        | How many MB of data were consumed during the time period?    |
| timestamp | Start timestamp within the time period                       |
| period    | ["1 hour", "1 day"] This indicates whether the current query is for a 1-hour dimension or a 1-day dimension. |