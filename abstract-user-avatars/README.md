# [Abstract User Avatars](https://www.abstractapi.com/api/user-avatar-api)

## __Description__
Create highly customizable avatar images with a person's name or initials to improve your user experience.

## __Example Request__
* Curl
```
curl "https://avatars.abstractapi.com/v1/?api_key={{token}}&name=John Smith"
```

* Raw
```
GET /v1/?api_key={{token}}&name=John%20Smith HTTP/1.1
Host: avatars.abstractapi.com
```

## __Response__
* Success
```
An image will appear with the letters "JS"
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