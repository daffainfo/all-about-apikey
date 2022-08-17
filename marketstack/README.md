# [Marketstack](https://marketstack.com/documentation)

## __Description__
Real-Time, Intraday & Historical Market Data API

## __Example Request__
* Curl
```
curl "https://api.marketstack.com/v1/eod?access_key={{token}}&symbols=AAPL"
```

* Raw
```
GET /v1/eod?access_key={{token}}&symbols=AAPL HTTP/1.1
Host: api.marketstack.com
...
```

## __Response__
* Success
```
{
    "pagination": {
        "limit": 100,
        "offset": 0,
        "count": 100,
        "total": 9944
    },
    "data": [
        {
            "open": 129.8,
            "high": 133.04,
            "low": 129.47,
            "close": 132.995,
            "volume": 106686703.0,
            "adj_high": 133.04,
            "adj_low": 129.47,
            "adj_close": 132.995,
            "adj_open": 129.8,
            "adj_volume": 106686703.0,
            "split_factor": 1.0,
            "dividend": 0.0,
            "symbol": "AAPL",
            "exchange": "XNAS",
            "date": "2021-04-09T00:00:00+0000"
            },
            [...]
    ]
}
```
* Error
```
{
    "error": {
        "code": "invalid_access_key",
        "message": "You have not supplied a valid API Access Key."
    }
}
```
## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
tue3sv9hzsey1me4l7fwq3t46u5k8wag
```
