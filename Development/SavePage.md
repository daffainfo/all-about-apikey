# [SavePage](https://docs.savepage.io/)

## __Description__
A free, RESTful API used to screenshot any desktop, or mobile website

## __Example Request__
* Curl
```
curl "https://api.savepage.io/v1?key={{token}}&q=https://www.google.com"
```

* Raw
```
GET /v1?key={{token}}&q=https://www.google.com HTTP/1.1
Host: api.savepage.io
```

## __Response__
* Success
```
Google image will appear
```
* Error
```
{
    "error":"461 - Cannot verify the API Key"
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
