# [IPFind](https://ipfind.io/documentation)

## __Description__
Geographic location of an IP address or any domain name along with some other useful information

## __Example Request__
* Curl
```
curl "https://app.ipfind.io/api/iplocation?apikey={{token}}"
```

* Raw
```
GET /api/iplocation?apikey={{token}} HTTP/1.1
Host: app.ipfind.io
```

## __Response__
* Success
```
{
    "continent": "North America",
    "country": "United States",
    "zipCode": "20149",
    "accuracyRadius": 1000,
    "flag": "https://ipfind.io/static/flags/us.png",
    "city": "Ashburn",
    "timezone": "America/New_York",
    "latitude": 39.0481,
    "countryGeoNameId": 6252001,
    ...
```
* Error
```
{
    "error": "Please ensure you've entered your token correctly.",
    "title": "Unknown Token"
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
