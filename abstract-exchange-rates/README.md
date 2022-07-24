# [Abstract Exchange Rates](https://www.abstractapi.com/api/exchange-rate-api)

## __Description__
Get live and historical data from 60+ fiat and crypto currencies via a modern REST API

## __Example Request__
* Curl
```
curl "https://currency.abstractapi.com/v1/?api_key={{token}}&base=USD"
```

* Raw
```
GET /v1/?api_key={{token}}&base=USD HTTP/1.1
Host: currency.abstractapi.com
```

## __Response__
* Success
```
{
    "base": "USD",
    "last_updated_unix": "1593614038",
    "last_updated_utc": "Wed, 01 Jul 2020 14:33:58 +0000",
    "exchange_rate": {
        "EUR": 0.889758,
        "CAD": 1.35676,
        "AUD": 1.44753,
        "GBP": 0.807175,
        "CHF": 0.946451,
        "CNY": 7.06409,
        ...
        ...
    }
}
```
* Error
```
{
    "error":{
        "message":"Invalid API key provided.",
        "code":"unauthorized",
        "details":null
    }
}
```

## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
of3ab02f3xd12ldofxc3fosc129sd241
```