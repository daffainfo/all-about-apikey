# [Scanii](https://docs.scanii.com/)

## __Description__
Simple REST API that can scan submitted documents/files for the presence of threats

## __Example Request__
* Curl
```
curl -u APIKEY:SECRETKEY https://api.scanii.com/v2.1/ping
```

* Raw
```
GET /v2.1/ping HTTP/1.1
Authorization: Basic QVBJS0VZOlNFQ1JFVEtFWQ==
Host: api.scanii.com
```

## __Response__
* Success
```
{
    "key" : "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
    "message" : "pong"
}
```
* Error
```
{
    "error" : "Apologies but we could not authenticate this request."
}
```

## __Regex__
* API Key
```
[a-z0-9]{32}
```
* Secret Key
```
[a-z0-9]{9}
```

## __Example key__
* API Key
```
tue3sv9hzsey1me4l7fwq3t46u5k8wag
```
* Secret Key
```
tue3sv9hzs
```