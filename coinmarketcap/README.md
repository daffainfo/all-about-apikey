# [CoinMarketCap](https://coinmarketcap.com/api/documentation/v1)

## __Description__
Cryptocurrencies Prices

## __Example Request__
* Curl
```
curl -H "X-CMC_PRO_API_KEY: {{token}}" https://pro-api.coinmarketcap.com/v1/cryptocurrency/listings/latest
```

* Raw
```
GET /v1/cryptocurrency/listings/latest HTTP/1.1
Host: pro-api.coinmarketcap.com
X-CMC_PRO_API_KEY: {{token}}
```

## __Response__
* Success
```
{
    "data": [
        {
            "id": 1,
            "name": "Bitcoin",
            "symbol": "BTC",
            "slug": "bitcoin",
            "cmc_rank": 5,
            "num_market_pairs": 500,
            "circulating_supply": 16950100,
            "total_supply": 16950100,
            "max_supply": 21000000,
            "last_updated": "2018-06-02T22:51:28.209Z",
            "date_added": "2013-04-28T00:00:00.000Z",
            "tags": [
                "mineable"
            ],
            "platform": null,
            "self_reported_circulating_supply": null,
            "self_reported_market_cap": null,
            "quote": {
                "USD": {
                    "price": 9283.92,
                    "volume_24h": 7155680000,
                    "volume_change_24h": -0.152774,
                    "percent_change_1h": -0.152774,
                    "percent_change_24h": 0.518894,
                    "percent_change_7d": 0.986573,
                    "market_cap": 852164659250.2758,
                    "market_cap_dominance": 51,
                    "fully_diluted_market_cap": 952835089431.14,
                    "last_updated": "2018-08-09T22:53:32.000Z"
                },
            ...
```
* Error
```
{
    "status": {
        "timestamp": "2022-04-17T06:58:28.344Z",
        "error_code": 1001,
        "error_message": "This API Key is invalid.",
        "elapsed": 0,
        "credit_count": 0
    }
}
```
## __Regex__
```
[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}
```

## __Example API key__
```
b54bcf4d-1bca-4e8e-9a24-22ff2c3d462c
```
