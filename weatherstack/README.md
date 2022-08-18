# [weatherstack](https://weatherstack.com/documentation)

## __Description__
Real-Time & Historical World Weather Data API

## __Example Request__
* Curl
```
curl "https://api.weatherstack.com/current?access_key={{token}}&query=New%20York"
```

* Raw
```
GET /current?access_key={{token}}&query=New%20York HTTP/1.1
Host: api.weatherstack.com
...
```

## __Response__
* Success
```
{
    "request": {
        "type": "City",
        "query": "New York, United States of America",
        "language": "en",
        "unit": "m"
    },
    "location": {
        "name": "New York",
        "country": "United States of America",
        "region": "New York",
        "lat": "40.714",
        "lon": "-74.006",
        "timezone_id": "America/New_York",
        "localtime": "2019-09-07 08:14",
        "localtime_epoch": 1567844040,
        "utc_offset": "-4.0"
    },
}
```
* Error
```
{
    "success": false,
    "error": {
        "code": 101,
        "type": "invalid_access_key",
        "info": "You have not supplied a valid API Access Key. [Technical Support: support@apilayer.com]"
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
