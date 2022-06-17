# [Browshot](https://browshot.com/api/documentation)

## __Description__
Easily make screenshots of web pages in any screen size, as any device

## __Example Request__
* Curl
```
curl "https://api.browshot.com/api/v1/simple?url=http://mobilito.net/&instance_id=12&width=640&height=480&key={{token}}"
```

* Raw
```
GET /api/v1/simple?url=http://mobilito.net/&instance_id=12&width=640&height=480&key={{token}} HTTP/1.1
Host: api.browshot.com
```

## __Response__
* Success
```
{
    "cost":0,
    "priority":1,
    "status":"in_queue",
    "url":"http://mobilito.net/",
    "id":"81830690"
}
```
* Error
```
{
    "error":"Wrong or missing API key"
}
```
## __Regex__
```
[a-zA-Z0-9]{27,30}
```

## __Example API key__
```
gLJALD3SH99MSsL5kC6mwuYtkviDvd
```
