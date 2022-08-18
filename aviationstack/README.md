# [aviationstack](https://aviationstack.com/documentation)

## __Description__
Real-time Flight Status & Global Aviation Data API

## __Example Request__
* Curl
```
curl "https://api.aviationstack.com/v1/flights?access_key={{token}}"
```

* Raw
```
GET /v1/flights?access_key={{token}} HTTP/1.1
Host: api.aviationstack.com
...
```

## __Response__
* Success
```
{
    "pagination": {
        "limit": 100,
        "offset": 0,
        "count": 100,
        "total": 1669022
    },
    "data": [
        {
            "flight_date": "2019-12-12",
            "flight_status": "active",
            "departure": {
                "airport": "San Francisco International",
                "timezone": "America/Los_Angeles",
                "iata": "SFO",
                "icao": "KSFO",
                "terminal": "2",
                "gate": "D11",
                ...
            }
        }
    ]
}
```
* Error
```
{
    "error": {
        "code": "invalid_access_key",
        "message": "You have not supplied a valid API Access Key."
    }
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
