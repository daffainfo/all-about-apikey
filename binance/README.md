# [Binance](https://github.com/binance/binance-spot-api-docs)

## __Description__
Exchange for Trading Cryptocurrencies based in China

## __Example Request__
* Curl
```
curl -H 'X-MBX-APIKEY: {{token}}' 'https://api.binance.com/api/v3/account'
```

* Raw
```
GET /api/v3/account HTTP/1.1
Host: api.binance.com
X-MBX-APIKEY: {{token}}
```

## __Response__
* Success
```
{
    "makerCommission": 15,
    "takerCommission": 15,
    "buyerCommission": 0,
    "sellerCommission": 0,
    "canTrade": true,
    "canWithdraw": true,
    "canDeposit": true,
    "updateTime": 123456789,
    "accountType": "SPOT",
    "balances": [
        {
        "asset": "BTC",
        "free": "4723846.89208129",
        "locked": "0.00000000"
        },
        {
        "asset": "LTC",
        "free": "4763368.68006011",
        "locked": "0.00000000"
        }
    ],
        "permissions": [
        "SPOT"
    ]
}
```
* Error
```
{
    "code":-2015,
    "msg":"Invalid API-key, IP, or permissions for action."
}
```
## __Regex__
```
[a-zA-Z0-9]{64}
```

## __Example API key__
```
8tc4fJ1ddM2VmnbFzTk3f7hXsrehnT8wP7u6EdIoVq7gyXWiL852TP1wnKp0qaGM
```
