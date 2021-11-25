# [Rijksmuseum](https://data.rijksmuseum.nl/user-generated-content/api//)

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