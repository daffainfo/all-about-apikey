# [Abstract Public Holidays](https://www.abstractapi.com/holidays-api)

## __Description__
Data on national, regional, and religious holidays via API

## __Example Request__
* Curl
```
curl "https://holidays.abstractapi.com/v1/?api_key={{token}}&country=GB&year=2021&month=1&day=25"
```

* Raw
```
GET /v1/?api_key={{token}}&country=GB&year=2021&month=1&day=25 HTTP/1.1
Host: holidays.abstractapi.com
```

## __Response__
* Success
```
{
    "total_count":1,
    "limit":100,
    "offset":0,
    "entries":[
        {
            "type":"collection",
            "name":"Favorites",
            "collection_type":"favorites",
            "id":"8830329105"
        }
    ]
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