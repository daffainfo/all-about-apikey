# [Cooper Hewitt](https://collection.cooperhewitt.org/api)

## __Description__
Smithsonian Design Museum

## __Example Request__
* Curl
```
curl -X GET "https://api.collection.cooperhewitt.org/rest/?method=api.spec.formats&access_token=ACCESS_TOKEN"
```

* Raw
```
GET /rest/?method=api.spec.formats&access_token=ACCESS_TOKEN HTTP/1.1
Host: api.collection.cooperhewitt.org
```

## __Response__
* Success
```
{
    "formats":["json","jsonp","dson"],
    "default_format":"json",
    "stat":"ok",
    "event_publishing_state":"ok"
}
```
* Error
```
{
    "error":{
        "code":400,
        "error":"Invalid access token",
        "message":"Invalid access token"
    },
    "stat":"error",
    "event_publishing_state":"ok"
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