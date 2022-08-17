# [Abstract Time, Date & Timezone](https://www.abstractapi.com/api/time-date-timezone-api)

## __Description__
Quickly and easily get the time and date of a location or IP address, or convert the time and date of one timezone into another

## __Example Request__
* Curl
```
curl "https://timezone.abstractapi.com/v1/current_time/?api_key={{token}}&location=Oxford, United Kingdom"
```

* Raw
```
GET /v1/current_time/?api_key={{token}}&location=Oxford,%20United%20Kingdom HTTP/1.1
Host: timezone.abstractapi.com
```

## __Response__
* Success
```
{
    "requested_location": "Oxford, United Kingdom",
    "longitude": -1.257677,
    "latitude": 51.752022,
    "datetime": "2020-07-01 14:22:13",
    "timezone_name": "British Summer Time",
    "timezone_abbreviation": "BST",
    "gmt_offset": "+1",
    "is_dst": true
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