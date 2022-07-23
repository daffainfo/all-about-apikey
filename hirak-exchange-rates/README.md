# [Hirak Exchange Rates](https://rates.hirak.site/)

## __Description__
Exchange rates between 162 currency & 300 crypto currency update each 5 min, accurate, no limits

## __Example Request__
* Curl
```
curl "https://rates.hirak.site/stat/?token={{token}}"
```

* Raw
```
GET /stat/?token={{token}} HTTP/1.1
Host: rates.hirak.site
```

## __Response__
* Success
```
{
    "token":"533d14f05aldo4k2m2eadumk4a4a21da",
    "plan":"trial",
    "hits":"Nothing found, do your first request!",
    "ordered":"19-04-2022 03:12:52",
    "expire":"20-05-2022 03:12:52",
    "total":0,
    "remain":50
}
```
* Error
```
{
    "result":"error",
    "message":"Token not valid"
}
```
## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
533d14f05aldo4k2m2eadumk4a4a21da
```
