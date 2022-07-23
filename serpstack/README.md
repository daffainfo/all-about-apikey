# [serpstack](https://serpstack.com/documentation)

## __Description__
Real-Time & Accurate Google Search Results API

## __Example Request__
* Curl
```
curl "http://api.serpstack.com/search?access_key={{token}}&query=mcdonalds"
```

* Raw
```
GET /search?access_key={{token}}&query=mcdonalds HTTP/1.1
Host: api.serpstack.com
```

## __Response__
* Success
```
{
    "request":{
        "success":true,
        "total_time_taken":1.1,
        "processed_timestamp":1655482312,
        "search_url":"http://www.google.com/search?q=mcdonalds\u0026gl=us\u0026hl=en\u0026safe=0\u0026num=10"
    },
    "search_parameters":{
        "engine":"google",
        "type":"web",
        "device":"desktop",
        "auto_location":"1",
        "google_domain":"google.com",
        "gl":"us",
        "hl":"en",
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
