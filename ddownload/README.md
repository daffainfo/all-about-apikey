# [ddownload](https://ddownload.com/api)

## __Description__
File Sharing and Storage

## __Example Request__
* Curl
```
curl "https://api-v2.ddownload.com/api/account/info?key={{token}}"
```

* Raw
```
GET /api/account/info?key={{token}} HTTP/1.1
Host: api-v2.ddownload.com
```

## __Response__
* Success
```
{
    "msg":"OK",
    "server_time":"2021-11-20 14:22:50",
    "status":200,
    "result":{
        "storage_left":"inf",
        "premium_traffic_left":0,
        "email":"example@gmail.com",
        "premium_expire":"2021-11-20 14:22:10",
        "balance":"0.00000",
        "traffic_used":"0",
        "traffic_left":"0",
        "storage_used":null
    }
}
```
* Error
```
{
    "msg":"Wrong auth",
    "server_time":"2021-11-20 14:25:18",
    "status":403
}
```

## __Regex__
```
[a-z0-9]{22}
```

## __Example API key__
```
of3ab02f3xd12ldofxc3fodadsadadad
```