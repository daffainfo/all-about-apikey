# Art-Design
List of Art and Design API

## Index
* [Cooper Hewitt](#1-cooper-hewitt)
* [Dribbble](#2-dribbble)
* [Rijksmuseum](#3-rijksmuseum)

# 1. [Cooper Hewitt](https://collection.cooperhewitt.org/api)

## __Description__
Smithsonian Design Museum

## __Example Request__
* Curl
```
curl -X GET "https://api.collection.cooperhewitt.org/rest/?method=api.spec.formats&access_token=ACCESS_TOKEN"
```

* Raw
```
GET /rest/?method=api.spec.formats&access_token=ACCESS_TOKEN HTTP/1.1
Host: api.collection.cooperhewitt.org
```

## __Response__
* Success
```
{
    "formats":["json","jsonp","dson"],
    "default_format":"json",
    "stat":"ok",
    "event_publishing_state":"ok"
}
```
* Error
```
{
    "error":{
        "code":400,
        "error":"Invalid access token",
        "message":"Invalid access token"
    },
    "stat":"error",
    "event_publishing_state":"ok"
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

# 2. [Dribbble](https://developer.dribbble.com/v2/)

## __Description__
Dribbble is a self-promotion and social networking platform for digital designers and creatives

## __Example Request__
* Curl
```
curl "https://api.dribbble.com/v2/user?access_token=ACCESS_TOKEN"
```

* Raw
```
GET /v2/user?access_token=ACCESS_TOKEN HTTP/1.1
Host: api.dribbble.com
```

## __Response__
* Success
```
{
    "id" : 1,
    "name" : "Dan Cederholm",
    "login" : "simplebits",
    "html_url" : "https://dribbble.com/simplebits",
    "avatar_url" : "https://d13yacurqjgara.cloudfront.net/users/1/avatars/normal/dc.jpg?1371679243",
    "bio" : "Co-founder &amp; designer of <a href=\"https://dribbble.com/dribbble\">@Dribbble</a>. Principal of SimpleBits. Aspiring clawhammer banjoist.",
    "location" : "Salem, MA",
    ....
```
* Error
```
{
    "message":"Bad credentials."
}
```

## __Regex__
```
[a-z0-9]{64}
```

## __Example API key__
```
om34l6c32snpjr1tsj7fixoexafrgr9i6023t2701yysa7fuqfbdgy0tct75gkeg
```

# 3. [Rijksmuseum](https://data.rijksmuseum.nl/user-generated-content/api//)

## __Description__
The Rijksmuseum is a Dutch national museum dedicated to arts and history in Amsterdam

## __Example Request__
* Curl
```
curl "https://www.rijksmuseum.nl/api/nl/usersets?key=APIKEY&format=json&page=2"
```

* Raw
```
GET /api/nl/usersets?key=APIKEY&format=json&page=2 HTTP/1.1
Host: www.rijksmuseum.nl
```

## __Response__
* Success
```
{
    "count": 1111111,
    "elapsedMilliseconds": 80,
    "userSets": [
        {"links": {
            "self": "https://www.rijksmuseum.nl/api/usersets/1111-mijn-eerste-verzameling",
            "web": "https://www.rijksmuseum.nl/nl/mijn/verzamelingen/11111--menno-baas/mijn-eerste-verzameling"},
            "id": "1111-mijn-eerste-verzameling",
            "count": 4,
            "type": "Default"
        }
    ]
}
```
* Error
```
{
    "message": "key not found"
} 
```

## __Regex__
```
[a-zA-Z0-9]{8}
```

## __Example API key__
```
Hs5yk0J3
```