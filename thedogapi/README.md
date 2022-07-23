# [TheDogApi](https://docs.thedogapi.com/)

## __Description__
Pictures of dogs from Tumblr

## __Example Request__
* Curl
```
curl --request GET \
    --url https://api.thedogapi.com/v1/votes \
    --header 'x-api-key: DEMO-API-KEY'
```

* Raw
```
GET /v1/votes HTTP/1.1
Host: api.thedogapi.com
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
[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[0-9a-f]{12}
```

## __Example API key__
```
da3ec69e-bdc3-8f07-b5e3-6521c026d4be
```