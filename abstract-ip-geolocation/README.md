# [Abstract IP Geolocation](https://www.abstractapi.com/api/ip-geolocation-api)

## __Description__
Get the location of any IP with a world-class APIserving city, region, country and lat/long data.

## __Example Request__
* Curl
```
curl "https://ipgeolocation.abstractapi.com/v1/?api_key={{token}}&ip_address=123.234.123.234"
```

* Raw
```
GET /v1/?api_key={{token}}&ip_address=123.234.123.234 HTTP/1.1
Host: ipgeolocation.abstractapi.com
```

## __Response__
* Success
```
{
    "ip": 92.184.105.98,
    "city": "Caen",
    "city_geoname_id": 3029241,
    "region": "Normandie",
    "region_iso_code": "FR-NOR",
    "region_geoname_id": 11071621,
    "postal_code": "14949",
    "country": "France",
    "country_code": "FR",
    "country_geoname_id": 3017382,
    "country_is_eu": true,
    "continent": "Europe",
    ...
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