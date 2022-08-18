# [ipapi](https://ipapi.com/documentation)

## __Description__
Real-time Geolocation & Reverse IP Lookup REST API

## __Example Request__
* Curl
```
curl "http://api.ipapi.com/api/161.185.160.93?access_key={{token}}"
```

* Raw
```
GET /api/161.185.160.93?access_key={{token}} HTTP/1.1
Host: api.ipapi.com
...
```

## __Response__
* Success
```
{
    "ip": "161.185.160.93",
    "hostname": "161.185.160.93",
    "type": "ipv4",
    "continent_code": "NA",
    "continent_name": "North America",
    "country_code": "US",
    "country_name": "United States",
    "region_code": "NY",
    "region_name": "New York",
    "city": "Brooklyn",
    "zip": "11238",
    "latitude": 40.676,
    "longitude": -73.9629,
    "location": {
        ...
    }
}
```
* Error
```
{
    "success":false,
    "error":{
        "code":101,
        "type":"invalid_access_key",
        "info":"You have not supplied a valid API Access Key. [Technical Support: support@apilayer.com]"
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
