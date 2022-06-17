# [AniAPI](https://aniapi.com/docs/authentication)

## __Description__
Anime discovery, streaming & syncing with trackers

## __Example Request__
* Curl
```
curl -i https://api.aniapi.com/v1/auth/me \
    -H "Authorization: Bearer <YOUR_JWT>"
```

* Raw
```
GET /v1/auth/me HTTP/1.1
Host: api.aniapi.com
Authorization: Bearer <YOUR_JWT>
```

## __Response__
* Success
```
{
    "status_code": 200,
    "message": "Hi Daffa",
    "data": {
        "username": "Daffa",
        "id": 1,
        //...
    },
    "version": "1"
}
```
* Error
```
{
    "status_code": 401,
    "message": "Unauthorized",
    "data": "Invalid Authorization header",
    "version": "1"
}
```

## __Regex__
```
^[A-Za-z0-9-_=]+\.[A-Za-z0-9-_=]+\.?[A-Za-z0-9-_.+/=]*$
```

## __Example API key__
```
eyJpc3MiOiJPbmxpbmUgSldUIEJ1aWxkZXIiLCJpYXQiOjE2M.jkxMDcxMjAsImV4cCI6MTY2MDY0MzEyMCwiYXVkIjo........
```