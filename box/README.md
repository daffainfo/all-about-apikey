# [Box](https://developer.box.com/)

## __Description__
File Sharing and Storage

## __Example Request__
* Curl
```
curl -X GET "https://api.box.com/2.0/collections" -H "Authorization: Bearer {{token}}"
```

* Raw
```
GET /2.0/collections HTTP/1.1
Host: api.box.com
Authorization: Bearer {{token}}
```

## __Response__
* Success
```
{
    "total_count":1,
    "limit":100,
    "offset":0,
    "entries":[{
            "type":"collection",
            "name":"Favorites",
            "collection_type":
            "favorites",
            "id":"8830329105"
        }
    ]
}
```
* Error
```

```
> No output if error

## __Regex__
```
[a-zA-Z0-9]{32}
```

## __Example API key__
```
OF3ab02f3cD12lDOfxc3foSg129sD241
```