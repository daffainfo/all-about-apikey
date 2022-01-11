# [Coinlib](https://coinlib.io/apidocs)

## __Description__
Crypto Currency Prices

## __Example Request__
* Curl
```
curl 'https://coinlib.io/api/v1/global?key={{token}}&pref=EUR'
```

* Raw
```
GET /api/v1/global?key={{token}}&pref=EUR HTTP/1.1
Host: coinlib.io
```

## __Response__
* Success
```
{
    "coins": 6656,
    "markets": 10170,
    "total_market_cap": "1465184971086.2172851562",
    "total_volume_24h": "15611208351.8629932404",
    "last_updated_timestamp": 1641782024,
    "remaining": 119
}
```
* Error
```
{
    "error":"Authentication failed."
}
```
## __Regex__
```
[a-z0-9]{16}
```

## __Example API key__
```
abcdefgh12345678
```
