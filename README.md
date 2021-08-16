# All About API

# 1. [TheCatApi](https://docs.thecatapi.com/)

## __Request__
* Curl
```
curl --request GET \
    --url https://api.thecatapi.com/v1/votes \
    --header 'x-api-key: DEMO-API-KEY'
```

* Raw
```
GET /v1/votes HTTP/1.1
Host: api.thecatapi.com
x-api-key: DEMO-API-KEY
```

## __Response__
* Success
```
[{
    "id": 31098,
    "image_id": "43u",
    "sub_id": null,
    "created_at": "2018-10-24T08:36:13.000Z",
    "value": 1,
    "country_code": null
}]
```
* Error
```
{
    "message": "AUTHENTICATION_ERROR - no valid x-api-key in header",
    "status": 401,
    "level": "info"
}
```

## __Regex__
```
[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[0-9a-z]{12}
```