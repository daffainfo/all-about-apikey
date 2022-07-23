# [Coinlayer](https://coinlayer.com/documentation)

## __Description__
Real-time Crypto Currency Exchange Rates

## __Example Request__
* Curl
```
curl 'https://api.coinlayer.com/live?access_key={{token}}'
```

* Raw
```
GET /live?access_key={{token}} HTTP/1.1
Host: api.coinlayer.com
```

## __Response__
* Success
```
{
    "success":true,
    "terms":"https:\/\/coinlayer.com\/terms",
    "privacy":"https:\/\/coinlayer.com\/privacy",
    "timestamp":1641304507,
    "target":"USD",
    "rates":{
        "ABC":00.00,
        "ACP":0.000000,
        "ACT":0.006995,
        ...
    }
}
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
of3ab02f3xd12ldofxc3fodadsadadad
```
