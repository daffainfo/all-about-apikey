# [positionstack](https://positionstack.com/documentation)

## __Description__
Accurate Forward & Reverse Batch Geocoding REST API

## __Example Request__
* Curl
```
curl "http://api.positionstack.com/v1/forward?access_key={{token}}&query=1600%20Pennsylvania%20Ave%20NW,%20Washington%20DC"
```

* Raw
```
GET /v1/forward?access_key={{token}}&query=1600%20Pennsylvania%20Ave%20NW,%20Washington%20DC HTTP/1.1
Host: api.positionstack.com
...
```

## __Response__
* Success
```
{
    "data": {
        "results": [
            {
                "latitude": 38.897675,
                "longitude": -77.036547,
                "label": "1600 Pennsylvania Avenue NW, Washington, DC, USA",
                "name": "1600 Pennsylvania Avenue NW",
                "type": "address",
                "number": "1600",
                "street": "Pennsylvania Avenue NW",
                "postal_code": "20500",
                "confidence": 1,
                "region": "District of Columbia",
                "region_code": "DC",
                "administrative_area": null,
                "neighbourhood": "White House Grounds",
                "country": "United States",
                "country_code": "US",
                "map_url": "http://map.positionstack.com/38.897675,-77.036547"
            }
        ]
    }
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
