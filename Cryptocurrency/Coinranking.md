# [Coinranking](https://developers.coinranking.com/api/documentation)

## __Description__
Live Cryptocurrency data

## __Example Request__
* Curl
```
curl "https://api.coinranking.com/v2/exchanges" -H "x-access-token: {{token}}"
```

* Raw
```
GET /v2/exchanges HTTP/1.1
Host: api.coinranking.com
x-access-token: {{token}}
```

## __Response__
* Success
```
{
    "status": "success",
    "data": {
        "stats": {
            "24hVolume": "6554685985.623574",
            "total": 198
        },
        "exchanges": [
            {
                "coinrankingUrl": "https://coinranking.com/exchange/-zdvbieRdZ+binance",
                "uuid": "-zdvbieRdZ",
                "name": "Binance",
                "iconUrl": "https://cdn.coinranking.com/mDTK5qrmq/binance.svg",
                "numberOfMarkets": 3,
                "24hVolume": "776337030.2052088",
                "rank": 1,
                "marketShare": "12.22",
                "verified": true,
                "recommended": true
            },
            {
                "coinrankingUrl": "https://coinranking.com/exchange/XHp8eCjIDc+zb",
                "uuid": "XHp8eCjIDc",
                "name": "ZB",
                "iconUrl": null,
                "lastTickerCreatedAt": 1546960123000,
                "numberOfMarkets": 128,
                "24hVolume": "693976176.906341",
                "rank": 2,
                "marketShare": "10.92",
                "verified": false,
                "recommended": false
            }
        ]
    }
}
```
* Error
```
{
    "status":"fail",
    "code":"UNAUTHORIZED",
    "message":"To use this endpoint please generate a free API key: https://developers.coinranking.com/create-account and upgrade to the right subscription plan: https://developers.coinranking.com/api/pricing"
}
```
## __Regex__
```
coinranking[a-z0-9]{48}
```

## __Example API key__
```
coinrankingabcdefghij12345abcw94d869bf2608a5aa76ba8aa7ede
```
