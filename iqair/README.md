# [IQAir](https://www.iqair.com/air-pollution-data-api)

## __Description__
Air quality and weather data

## __Example Request__
* Curl
```
curl "http://api.airvisual.com/v2/countries?key={{token}}"
```

* Raw
```
GET /v2/countries?key={{token}} HTTP/1.1
Host: api.airvisual.com
```

## __Response__
* Success
```
{
    "status":"success",
    "data":[
        {"country":"Afghanistan"},
        {"country":"Albania"},
        {"country":"Algeria"},
        {"country":"Andorra"},
        {"country":"Angola"}
        ...
    ]
}
```
* Error
```
{
    "status":"fail",
    "data":{
        "message":"Forbidden"
    }
}
```
## __Regex__
```
[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}
```

## __Example API key__
```
abcd1234-abcd-1234-abcd-abcd1234abcd
```