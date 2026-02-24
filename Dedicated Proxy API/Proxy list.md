# Proxy list

**Path:** /ip/open-api/proxy-list

**Method:** GET

**Interface description: Query purchased proxies**

Parameter description:

| Parameter name | Is it required | Example | Remarks                                | Usage scenarios |
| -------------- | -------------- | ------- | -------------------------------------- | --------------- |
| proxy_ids      | No             | i14iudm | Proxy ID, multiple separated by commas |                 |
| page           | Yes            | 1       | Page number                            |                 |
| page_size      | Yes            | 10      | Number of proxies per page <= 50       |                 |

 

**Return data:**

```javascript
 {
  "data": {
    "list": [
      {
        "id": "i14isvi",
        "host": "45.199.6.53",
        "public_ip": "45.199.6.53",
        "port": "45001",
        "type": "socks5",
        "area_id": "27",
        "user": "odO652e60f0ab895",
        "password": "p6FNdAze4EhnOT8WUg",
        "auto_extend": "1",
        "expire_time": "1701599163",
        "buy_time": "1699007163",
        "country_code": "CL",
        "ip_type": "STATIC_DATACENTER",
        "ip_version": "IPv4",
        "renewal_time":"1768779904"
      }
    ],
    "total": 1,
    "page": 1,
    "page_size": 50
  },
  "code": 0,
  "msg": "Success"
}
```

 

Field Description:

| id           | Proxy ID                                                     |
| ------------ | ------------------------------------------------------------ |
| host         | Connect to host                                              |
| port         | port                                                         |
| public_ip    | Egress IP                                                    |
| type         | Protocol type socks5 ssh http                                |
| area_id      | Region ID                                                    |
| user         | account                                                      |
| password     | password                                                     |
| auto_extend  | Whether to enable automatic renewal: 1 for yes, 0 for no     |
| expire_time  | Valid time, timestampDue to asynchronous processing, the updated expiration date will only be displayed once the renewal is fully completed. |
| country_code | Country code: US                                             |
| ip_version   | IP version: IPv4 IPv6                                        |
| ip_type      | Proxy type: STATIC_DATACENTER static data center STATIC_ISP static residential STATIC_ISP_PRO static residential pro |
| buy_time     | Purchase time, timestamp                                     |
| renewal_time | Last completed renewal date                                  |