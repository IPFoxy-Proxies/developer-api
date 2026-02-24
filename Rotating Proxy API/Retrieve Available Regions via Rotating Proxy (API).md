# Retrieve Available Regions via Rotating Proxy (API)

**The list of available residential areas can be obtained via the following API:**

**Path:** /ip/open-api/dynamic-user-region

**Method:** GET

**Interface Description: Retrieves a list of regions where rotating residential proxies are available.**

**Returned data:**

```javascript
 {
    "data": {
            "country": "Bengal",
            "country_code": "BD",
            "state_code": "Dhaka",
            "city_code": "Dhaka"
    },
    "code": 0,
    "msg": "Success"
}
```

Field description:

| Field Name   | Description          |
| ------------ | -------------------- |
| country_code | Country Code         |
| state_code   | State/Province Codes |
| city_code    | City Code            |
| country      | nation               |