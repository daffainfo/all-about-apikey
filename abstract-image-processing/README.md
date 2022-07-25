# [Abstract Image Processing](https://www.abstractapi.com/api/image-processing-optimization-api)

## __Description__
Manage your images programmatically with this powerful API: compress, convert, crop, resize, and more.

## __Example Request__
* Curl
```
curl https://images.abstractapi.com/v1/url/ -X POST -H "Content-Type: application/json" -H "Accept: application/json" -d '{"api_key": "{{token}}", "lossy": true, "url": "https://s3.amazonaws.com/static.abstractapi.com/test-images/dog.jpg"}
```

* Raw
```
POST https://images.abstractapi.com/v1/url/ HTTP/1.1
Host: images.abstractapi.com
Content-Type: application/json
Accept: application/json

{"api_key": "{{token}}", "lossy": true, "url": "https://s3.amazonaws.com/static.abstractapi.com/test-images/dog.jpg"}
```

## __Response__
* Success
```
{
    "original_size":205559,
    "original_height":430,
    "original_width":1142,
    "final_size":75101,
    "bytes_saved":130458,
    "final_height":430,
    "final_width":1142,
    "url":"https://abstr..."
}
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