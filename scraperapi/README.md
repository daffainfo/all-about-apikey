# [ScraperAPI](https://www.scraperapi.com/documentation/)

## __Description__
Easily build scalable web scrapers

## __Example Request__
* Curl
```
curl "http://api.scraperapi.com/account?api_key={{token}}"
```

* Raw
```
GET /account?api_key={{token}} HTTP/1.1
Host: api.scraperapi.com
```

## __Response__
* Success
```
{
    "burst":0,
    "concurrencyLimit":5,
    "concurrentRequests":0,
    "failedRequestCount":1,
    "requestCount":401,
    "requestLimit":1000
}
```
* Error
```
Unauthorized request, please make sure your API key is valid.
```
## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
tue3sv9hzsey1me4l7fwq3t46u5k8wag
```
