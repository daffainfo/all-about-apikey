# [CurrencyScoop](https://currencyscoop.com/api-documentation)

## __Description__
Real-time and historical currency rates JSON API

## __Example Request__
* Curl
```
curl "https://api.currencyscoop.com//v1/historical?api_key={{token}}&date=2022-01-01"
```

* Raw
```
GET /v1/historical?api_key={{token}}&date=2022-01-01 HTTP/1.1
Host: api.currencyscoop.com
```

## __Response__
* Success
```
{
    "meta":{
        "code":200,
        "disclaimer":"Usage subject to terms: https:\/\/currencyscoop.com\/terms"},
        "response":{
            "date":"2022-01-01",
            "base":"USD",
            "rates":{
                "AED":3.6725,
                "AFN":103.73042093,
                "ALL":106.23967243,
                "AMD":479.91721441,
                "ANG":1.78750007
                ...
```
* Error
```
{
    "meta":{
        "code":401,
        "error_type":"auth failed",
        "error_detail":"Missing or invalid api credentials. See https:\/\/currencyscoop.com\/api for details."
    },
    "response":[]
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
