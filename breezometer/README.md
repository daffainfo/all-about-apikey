# [BreezoMeter](https://docs.breezometer.com/)

## __Description__
Location-based Air Pollution, Pollen & Active Fires information enables businesses to develop solutions that help reduce exposure to environmental hazards.

## __Example Request__
* Curl
```
curl "https://api.breezometer.com/air-quality/v2/current-conditions?lat=48.857456&lon=2.354611&key={{token}}"
```

* Raw
```
GET /air-quality/v2/current-conditions?lat=48.857456&lon=2.354611&key={{token}} HTTP/1.1
Host: api.breezometer.com
```

## __Response__
* Success
```
{
    "metadata": null,
    "data":{
        "datetime": "2022-08-17T11:00:00Z",
        "data_available": true,
        "indexes":{
            "baqi": {
                "display_name": "BreezoMeter AQI",
                "aqi": 65,
                "aqi_display": "65",
                "color": "#A2DB26",
                "category": "Good air quality",
                "dominant_pollutant": "o3"
            }
        }
    },
    "error": null
}
```
* Error
```
{
    "metadata":null,
    "data":null,
    "error":{
        "code":"invalid_api_key",
        "title":"Invalid API key",
        "detail":"Provided API key is invalid. Check for accidental whitespace characters and note that the key is case sensitive"
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