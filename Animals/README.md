# Animals
List of animals API

## Index
* [TheCatApi](#1-thecatapi)
* [IUCN](#2-iucn)

# 1. [TheCatApi](https://docs.thecatapi.com/)

## __Description__
Pictures of cats from Tumblr

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

## __Example API key__
```
0r98cr1s-9xef-m1ae-vk3o-vk2ld01c9v98
```

# 2. [IUCN](http://apiv3.iucnredlist.org/api/v3/docs)

## __Description__
IUCN Red List of Threatened Species

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

## __Example API key__
```
wrion7bk4lh7pxp2wiq57mjak6s0tp34fj1fiemdjqj1g5xl57hi3km8g6jpv28z
```