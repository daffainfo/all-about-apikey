# [CloudConvert](https://cloudconvert.com/api/v2)

## __Description__
Online file converter for audio, video, document, ebook, archive, image, spreadsheet, presentation

## __Example Request__
* Curl
```
curl "https://api.cloudconvert.com/v2/tasks" -H "Authorization: Bearer {{token}}"
```

* Raw
```
GET /v2/tasks HTTP/1.1
Host: api.cloudconvert.com
Authorization: Bearer {{token}}
```

## __Response__
* Success
```
{
    "data":[],
    "links":{
        "first":"https:\/\/api.cloudconvert.com\/v2\/tasks?page=1",
        "last":null,
        "prev":null,
        "next":null
    },
    "meta":{
        "current_page":1,
        "from":null,
        "path":"https:\/\/api.cloudconvert.com\/v2\/tasks",
        "per_page":100,
        "to":null
    }
}
```
* Error
```
{
    "message":"Unauthenticated.",
    "code":"UNAUTHENTICATED"
}
```
## __Regex__
```
^[A-Za-z0-9-_=]+\.[A-Za-z0-9-_=]+\.?[A-Za-z0-9-_.+/=]*$
```

## __Example API key__
```
eyJpc3MiOiJPbmxpbmUgSldUIEJ1aWxkZXIiLCJpYXQiOjE2M.jkxMDcxMjAsImV4cCI6MTY2MDY0MzEyMCwiYXVkIjo........
```
