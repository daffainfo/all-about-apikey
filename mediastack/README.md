# [mediastack](https://mediastack.com/documentation)

## __Description__
Free, Simple REST API for Live News & Blog Articles

## __Example Request__
* Curl
```
curl "https://api.mediastack.com/v1/news?access_key={{token}}&keywords=tennis&countries=us,gb,de"
```

* Raw
```
GET /v1/news?access_key={{token}}&keywords=tennis&countries=us,gb,de HTTP/1.1
Host: api.mediastack.com
...
```

## __Response__
* Success
```
{
    "pagination": {
        "limit": 100,
        "offset": 0,
        "count": 100,
        "total": 293
    },
    "data": [
        {
            "author": "TMZ Staff",
            "title": "Rafael Nadal Pulls Out Of U.S. Open Over COVID-19 Concerns",
            "description": "Rafael Nadal is officially OUT of the U.S. Open ... the tennis legend said Tuesday it's just too damn unsafe for him to travel to America during the COVID-19 pandemic. \"The situation is very complicated worldwide,\" Nadal wrote in a statement. \"The…",
            "url": "https://www.tmz.com/2020/08/04/rafael-nadal-us-open-tennis-covid-19-concerns/",
            ...
        }
    ]
}
```
* Error
```
{
    "error": {
        "code": "invalid_access_key",
        "message": "You have not supplied a valid API Access Key."
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
