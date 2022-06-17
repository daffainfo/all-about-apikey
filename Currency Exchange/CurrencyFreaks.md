# [CurrencyFreaks](https://currencyfreaks.com/documentation.html)

## __Description__
Provides current and historical currency exchange rates with free plan 1K requests/month

## __Example Request__
* Curl
```
curl "https://api.currencyfreaks.com/latest?apikey={{token}}"
```

* Raw
```
GET /latest?apikey={{token}} HTTP/1.1
Host: api.currencyfreaks.com
```

## __Response__
* Success
```
{
    "date":"2022-06-17 00:05:00+00",
    "base":"USD",
    "rates":{
        "AGLD":"3.6231884057971016",
        "FJD":"2.1725358446689014",
        "MATIC":"2.6260504201680672",
        "MXN":"20.424",
        "STD":"23263.0",
        ...
```
* Error
```
{
    "success":false,
    "error":{
        "status":"404",
        "message":"You have not supplied a valid apikey. Contact tech. support for assistance at support@currencyfreaks.com"
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
