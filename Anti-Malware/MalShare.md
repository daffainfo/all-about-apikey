# [MalShare](https://malshare.com/doc.php)

## __Description__
Malware Archive / file sourcing

## __Example Request__
* Curl
```
curl https://api.malshare.com/api.php?api_key=YOURAPIKEY&action=getlist
```

* Raw
```
GET /api.php?api_key=YOURAPIKEY&action=getlist HTTP/1.1
Host: api.malshare.com
```

## __Response__
* Success
```
[
    {
        "md5":"cd25ad16a214e03b50e6d56d05e45e16",
        "sha1":"33910b305bb460c3a1fa0b1c2dbae19f9eaf3ce5","sha256":"e5b6c1fad3ced7fd27922507d739fe7113e466eb155438c48f8b7aea24359d22"
    },
    ...
]
```
* Error
```
Error 14000 (Account not activated)
```

## __Regex__
```
[a-z0-9]{64}
```

## __Example API key__
```
tue3sv9hzsey1me4l7fwq3t46u5k8wagtue3sv9hzsey1me4l7fwq3t46u5k8wag
```