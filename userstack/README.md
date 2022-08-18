# [userstack](https://userstack.com/documentation)

## __Description__
Secure User-Agent String Lookup JSON API

## __Example Request__
* Curl
```
curl "https://api.userstack.com/api/detect?access_key={{token}}"
```

* Raw
```
GET /api/detect?access_key={{token}} HTTP/1.1
Host: api.userstack.com
...
```

## __Response__
* Success
```
{
    "ua": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/71.0.3578.98 Safari/537.36",
    "type": "browser",
    "brand": "Apple",
    "name": "Mac",
    "url": "https://www.google.com/about/company/",
    "os": {
        "name": "macOS 10.14 Mojave",
        "code": "macos_10_14",
        ...
    }
}
```
* Error
```
{
    "success": false,
    "error": {
        "code": 101,
        "type": "invalid_access_key",
        "info": "You have not supplied a valid API Access Key. [Technical Support: support@apilayer.com]"
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
