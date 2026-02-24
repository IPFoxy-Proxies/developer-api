# Use instruction

The API request path is: https://apis.ipfoxy.com

The request header always contains `api-token（proxy token` ,`api-id（user ID）`

post request with form-data format

The request frequency for a single account is limited to 60 times in 1 minute

> **Scope of use of the API：** Currently support dedicated proxy API purchase, proxy region query, purchase proxy, renew proxy, view account information, view order information, view proxy list, view order price and other functions.
>
> rotating proxies integration method please[ **click here to go** ](https://help.ipfoxy.com/docs/1eyfJt).

 

Dedicated Proxy API Result Code:

| 0     | Success                            |
| ----- | ---------------------------------- |
| 60400 | Parameter error                    |
| 60401 | Authorization failed               |
| 60300 | Insufficient balance               |
| 60500 | Service error                      |
| 60600 | The proxy does not support renewal |
| 17003 | Wrong purchase quantity            |
| 17019 | Proxy sold out or out of stock     |
| 17012 | Proxy out of stock                 |
| 17001 | Purchase is not supported          |
| 17002 | Wrong valid duration               |
| 17011 | The proxy has been removed         |
| 17004 | Proxy expired or unassigned        |
| 10086 | Request Error                      |
| 8700  | Order Failed (suggest retrying)    |
| 50000 | Request Rate Limit Exceeded        |