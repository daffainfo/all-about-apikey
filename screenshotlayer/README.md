# [screenshotlayer](https://screenshotlayer.com/documentation)

## __Description__
URL 2 Image

## __Example Request__
* Curl
```
curl "http://api.screenshotlayer.com/api/capture?access_key={{token}}&url=http%3A%2F%2Fgoogle.com"
```

* Raw
```
GET /api/capture?access_key={{token}}&url=http%3A%2F%2Fgoogle.com HTTP/1.1
Host: api.screenshotlayer.com
...
```

## __Response__
* Success
```
Google image will appear
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
