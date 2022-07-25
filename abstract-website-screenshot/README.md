# [Abstract Website Screenshot](https://www.abstractapi.com/api/website-screenshot-api)

## __Description__
Transform any URL into an image with Abstract's Website Screenshot API

## __Example Request__
* Curl
```
curl "https://screenshot.abstractapi.com/v1/?api_key={{token}}&url=https://www.apple.com" -o example.jpg
```

* Raw
```
GET /v1/?api_key={{token}}&url=https://www.apple.com HTTP/1.1
Host: screenshot.abstractapi.com
```

## __Response__
* Success
```
The screenshot image will appear
```
* Error
```
{
    "error":{
        "message":"Invalid API key provided.",
        "code":"unauthorized",
        "details":null
    }
}
```

## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
of3ab02f3xd12ldofxc3fosc129sd241
```