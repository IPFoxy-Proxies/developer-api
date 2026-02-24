# Region Query

**Path:** /ip/open-api/area-list

**Method:** GET

**Interface description: Used to check and obtain** **a list of proxy region that can be purchased**

**Response:**

```javascript
{
  "data": [
    {
      "id": "179",
      "ip_type": "STATIC_DATACENTER",
      "status": "true",
      "ip_version": "IPv4",
      "country": "United States",
      "country_code": "US",
      "region": "Zone D"
    },
    {
      "id": "159",
      "ip_type": "STATIC_DATACENTER",
      "status": "true",
      "ip_version": "IPv6",
      "country": "United States",
      "country_code": "US",
      "region": "Zone IPv6"
    },
    {
      "id": "174",
      "ip_type": "STATIC_ISP",
      "status": "true",
      "ip_version": "IPv4",
      "country": "United States",
      "country_code": "US",
      "region": "Residential"
    }
  ],
  "code": 0,
  "msg": "Success"
}
```

 

Field description:

| id           | Proxy region ID                                              |
| ------------ | ------------------------------------------------------------ |
| ip_type      | Proxy type: STATIC_DATACENTER static data center STATIC_ISP static residential  STATIC_ISP_PRO static residential pro |
| status       | Status: true on sale; false sold out/removed                 |
| ip_version   | IP version: IPv4  IPv6                                       |
| country      | Country: United States, United Kingdom                       |
| country_code | Country code: US                                             |
| region       | Available Zone: Zone A  Zone B Residential                   |