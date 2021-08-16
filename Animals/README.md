# Animals
list of animals API

# [TheCatApi](https://docs.thecatapi.com/)

## __Example Request__
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

# [IUCN](http://apiv3.iucnredlist.org/api/v3/docs)

## __Example Request__
* Curl
```
curl --request GET \
    --url http://apiv3.iucnredlist.org/api/v3/country/list?token=API-KEY
```

* Raw
```
GET /api/v3/country/list?token=API-KEY HTTP/1.1
Host: apiv3.iucnredlist.org
```

## __Response__
* Success
```
{"count":251,"results":[{"isocode":"UZ","country":"Uzbekistan"},{"isocode":"QA","country":"Qatar"}....]
```
* Error
```
{
    "message":"Token not valid!"
}
```

## __Regex__
```
[a-z0-9]{64}
```
