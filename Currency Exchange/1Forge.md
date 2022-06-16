# [1Forge](https://1forge.com/api)

## __Description__
Forex currency market data

## __Example Request__
* Curl
```
curl "https://api.1forge.com/quota?api_key={{token}}"
```

* Raw
```
GET /quota?api_key={{token}} HTTP/1.1
Host: api.1forge.com
```

## __Response__
* Success
```
{
    quota_used: 259,
    quota_limit: 5000,
    quota_remaining: 4741,
    hours_until_reset: 23
}
```
* Error
```
{
    "error":true,
    "message":"API Key Not Valid. Please go to 1forge.com to get an API key. If you have any questions please email us at contact@1forge.com"
}
```
## __Regex__
```
[a-zA-Z0-9]{32}
```

## __Example API key__
```
QSzFlcDwaXtfevSu4Oo98AsJb4fKMGio
```
