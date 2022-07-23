# [IUCN](http://apiv3.iucnredlist.org/api/v3/docs)

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