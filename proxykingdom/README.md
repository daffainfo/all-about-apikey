# [ProxyKingdom](https://proxykingdom.com/documentation)

## __Description__
Rotating Proxy API that produces a working proxy on every request

## __Example Request__
* Curl
```
curl "https://api.proxykingdom.com/proxy?token={{token}}"
```

* Raw
```
GET /proxy?token={{token}} HTTP/1.1
Host: api.proxykingdom.com
```

## __Response__
* Success
```
{
    "address": "123.123.123.123",
    "port": 8080,
    "protocol": "Http",
    "accessType": "Elite",
        "cityName": null,
        "postalCode": null,
        "latitude": 1,
        "longitude": 1,
        "accuracyRadius": 1,
        "timezone": null,
        "country": null,
        "continent": null,
        "subdivisions": []
    },
    "lastTested": "2022-06-17T12:00:48Z"
}
```
* Error
```
{
    "pc_status":403,
    "error":"Token is invalid or account is temporarily blocked! please login to your dashboard for more details"
}
```
## __Regex__
```
[a-zA-Z0-9_]{22}
```

## __Example API key__
```
kuEkyhxkL2ckwS_YM3wORg
```