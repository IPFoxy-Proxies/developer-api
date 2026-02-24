Rotating proxy resellers must first read the 👉 [**Access Pre-Instruction Document**](https://www.ipfoxy.com/help/docs/jie-ru-qian-zhi-shuo-ming-wen-dang-bi-kan) and complete the **API access application and registration** process.
Once approved, you will be able to obtain Rotating Proxy line Regions via the following API:

**Path:** /ip/open-api/get-region-list

**Method:** GET

**Interface description: Rotating proxy reseller acquisition supports dynamic line areas**

**Return data:**

```javascript
 {
  "data": [
    {
      "val_cn": "美国",
      "val_en": "United States",
      "val_ru": "Соединенные Штаты",
      "val_tc": "美國",
      "country_code": "US",
      "childs": [
        {
          "proxy_val": "Illinois",
          "val": "Illinois",
          "mode": ["1", "2"],
          "childs": [
            {
              "country_code": "US",
              "proxy_val": "Elgin",
              "val": "Elgin",
              "mode": ["1", "2"]
            },
            {
              "country_code": "US",
              "proxy_val": "Mountprospect",
              "val": "Mountprospect",
              "mode": ["1", "2"]
            }
          ]
        }
      ]
    }
  ],
  "code": 0,
  "msg": "Success"
}
```

Field Description:

| val_cn              | Chinese                       |
| ------------------- | ----------------------------- |
| val_en              | English                       |
| val_ru              | Russian                       |
| val_tc              | Traditional Chinese           |
| country_code        | Country code                  |
| data[].val          | State/Province                |
| data[].childs[].val | City                          |
| mode                | 1: Stickiness 2: Each request |