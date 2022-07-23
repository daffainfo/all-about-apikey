# [ApiFlash](https://apiflash.com/)

## __Description__
Chrome based screenshot API for developers

## __Example Request__
* Curl
```
curl "https://api.apiflash.com/v1/urltoimage?access_key={{token}}&url=https://google.com"
```

* Raw
```
GET /v1/urltoimage?access_key={{token}}&url=https://google.com HTTP/1.1
Host: api.apiflash.com
```

## __Response__
* Success
```
Google image will appear
```
* Error
```
No access key was provided.
```
## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
tue3sv9hzsey1me4l7fwq3t46u5k8wag
```
