# Anime
List of anime API

## Index
* [AniAPI](#1-aniapi)
* [MyAnimeList](#2-myanimelist)

# 1. [AniAPI](https://aniapi.com/docs/authentication)

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

# 2. [MyAnimeList](https://myanimelist.net/apiconfig/references/api/v2)

## __Description__
Anime and Manga Database and Community

## __Example Request__
* Curl
```
curl 'https://api.myanimelist.net/v2/anime?q=one&limit=4' \
-H 'Authorization: Bearer YOUR_TOKEN'
```

* Raw
```
GET /v2/anime?q=one&limit=4 HTTP/1.1
Host: api.myanimelist.net
Authorization: Bearer YOUR_TOKEN
```

## __Response__
* Success
```
{
  "data": [
    {
      "node": {
        "id": 459,
        "title": "One Piece Movie 1",
        "main_picture": {
          "medium": "https://myanimelist.cdn-dena.com/images/anime/5/20925.jpg",
          "large": "https://myanimelist.cdn-dena.com/images/anime/5/20925l.jpg"
        }
      }
    }
  ],
  "paging": {
    "next": "https://api.myanimelist.net/v2/anime?offset=4&q=one&limit=4"
  }
}
```
* Error
```
{
    "error": "invalid_token"
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