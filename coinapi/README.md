# [CoinAPI](https://docs.coinapi.io/)

## __Description__
All Currency Exchanges integrate under a single api

## __Example Request__
* Curl
```
curl https://rest.coinapi.io/v1/exchanges --request GET --header "X-CoinAPI-Key: {{token}}"
```

* Raw
```
GET /v1/exchanges HTTP/1.1
Host: rest.coinapi.io
X-CoinAPI-Key: {{token}}
```

## __Response__
* Success
```
[
    {
        "exchange_id": "OKCOIN_CNY",
        "website": "https://www.okcoin.cn/",
        "name": "OKCoin CNY",
        "data_start": "2013-06-12",
        "data_end": "2018-03-09",
        "data_quote_start": "2015-02-15T12:53:50.3430000Z",
        "data_quote_end": "2018-03-09T23:34:52.5800000Z",
        "data_orderbook_start": "2015-02-15T12:53:50.3430000Z",
        "data_orderbook_end": "2018-03-09T23:34:52.5800000Z",
        "data_trade_start": "2013-06-12T14:24:24.0000000Z",
        "data_trade_end": "2017-11-01T16:30:39.7077259Z",
        "data_symbols_count": 2,
        "volume_1hrs_usd": 0.0,
        "volume_1day_usd": 0.0,
        "volume_1mth_usd": 0.0
    },
    {
        "exchange_id": "HUOBI",
        "website": "https://www.huobi.com/",
        "name": "Huobi (HBUS)",
        "data_start": "2015-03-29",
        "data_end": "2019-11-03",
        "data_quote_start": "2015-03-29T21:46:06.2630000Z",
        "data_quote_end": "2019-11-03T18:22:29.1837496Z",
        "data_orderbook_start": "2015-03-29T21:46:06.2630000Z",
        "data_orderbook_end": "2019-11-03T18:23:53.2859878Z",
        "data_trade_start": "2015-03-29T21:46:08.7030000Z",
        "data_trade_end": "2019-11-03T18:21:48.2770000Z",
        "data_symbols_count": 403,
        "volume_1hrs_usd": 1605.80,
        "volume_1day_usd": 59957.44,
        "volume_1mth_usd": 1259508.43
    }
]
```
* Error
```
{
    "error": "Invalid API key. If this is a new API Key, then we need a few minutes to propagate the new key through our independent server sites. This behavior is by design as our multiple geographical independent sites are designed to be highly available, and we didn\u0027t have a single point where the API keys are stored."
}
```
## __Regex__
```
[A-Z0-9]{8}-[A-Z0-9]{4}-[A-Z0-9]{4}-[A-Z0-9]{4}-[A-Z0-9]{12}
```

## __Example API key__
```
ABCD1234-ABCD-1234-ABCD-ABCDEFGH1234
```
