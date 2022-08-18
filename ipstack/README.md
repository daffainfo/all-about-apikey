# [ipstack](https://ipstack.com/documentation)

## __Description__
Locate and identify website visitors by IP address

## __Example Request__
* Curl
```
curl "https://api.ipstack.com/134.201.250.155?access_key={{token}}"
```

* Raw
```
GET /134.201.250.155?access_key={{token}} HTTP/1.1
Host: api.ipstack.com
...
```

## __Response__
* Success
```
{
    "ip": "134.201.250.155",
    "hostname": "134.201.250.155",
    "type": "ipv4",
    "continent_code": "NA",
    "continent_name": "North America",
    "country_code": "US",
    "country_name": "United States",
    "region_code": "CA",
    ...
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
