# [Currencylayer](https://currencylayer.com/documentation)

## __Description__
Exchange rates and currency conversion

## __Example Request__
* Curl
```
curl "http://api.currencylayer.com/live?access_key={{token}}"
```

* Raw
```
GET /live?access_key={{token}} HTTP/1.1
Host: api.currencylayer.com
```

## __Response__
* Success
```
{
    "success":true,
    "terms":"https:\/\/currencylayer.com\/terms",
    "privacy":"https:\/\/currencylayer.com\/privacy",
    "timestamp":1655367183,
    "source":"USD",
    "quotes":{
        "USDAED":3.673101,
        "USDAFN":89.48456,
        "USDALL":114.624638,
        "USDAMD":424.067918,
        "USDANG":1.807216
        ...
```
* Error
```
{
    "success":false,
    "error":{
        "code":101,
        "type":"invalid_access_key",
        "info":"You have not supplied a valid API Access Key. [Technical Support: support@apilayer.com]"
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
