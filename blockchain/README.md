# [Blockchain](https://www.blockchain.com/api)

## __Description__
Bitcoin Payment, Wallet & Transaction Data

## __Example Request__
* Curl
```
curl 'https://api.blockchain.com/v3/exchange/accounts' -H 'X-API-Token: {{token}}'
```

* Raw
```
GET /v3/exchange/accounts HTTP/1.1
Host: api.blockchain.com
X-API-Token: {{token}}
```

## __Response__
* Success
```
{
    "primary": [
        {
        "currency": "BTC",
        "balance": 0.00366963,
        "available": 0.00266963,
        "balance_local": 38.746779155,
        "available_local": 28.188009155,
        "rate": 10558.77
        }
    ],
    "additionalProp1": [
        {
        "currency": "BTC",
        "balance": 0.00366963,
        "available": 0.00266963,
        "balance_local": 38.746779155,
        "available_local": 28.188009155,
        "rate": 10558.77
        }
    ],
    ...
}
```
* Error
```
{
    "timestamp":"2022-01-04T15:08:26.723+00:00",
    "status":401,
    "error":"Unauthorized",
    "message":"",
    "path":"/accounts"
}
```

## __Regex__
```
[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[0-9a-f]{12}
```

## __Example API key__
```
da3ec69e-bdc3-8f07-b5e3-6521c026d4be
```
