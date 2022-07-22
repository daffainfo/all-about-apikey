# [Asana](https://developers.asana.com/docs/overview)

## __Description__
Programmatic access to all data in your asana system

## __Example Request__
* Curl
```
curl https://app.asana.com/api/1.0/users/me -H "Authorization: Bearer {{token}}"
```

* Raw
```
GET /api/1.0/users/me HTTP/1.1
Host: app.asana.com
Authorization: Bearer {{token}}
...
```

## __Response__
* Success
```
{
    "data":{
        "gid":"123456789023456",
        "email":"test@gmail.com",
        "name":"Test",
        "photo":null,
        "resource_type":"user",
        "workspaces": [
            {
                "gid":"123456789023456",
                "name":"Test",
                "resource_type":"workspace"
            },
            {
                "gid":"123456789023456",
                "name":"emailDomain",
                "resource_type":"workspace"
            }
        ]
    }
}
```
* Error
```
{
    "errors":[
        {
            "message":"Not Authorized",
            "help":"For more information on API status codes and how to handle them, read the docs on errors: https://asana.com/developers/documentation/getting-started/errors"
        }
    ]
}
```
## __Regex__
```
0\/[a-z0-9]{32}
```

## __Example API key__
```
0/123aa4df560cdb7890f123spd1p2ep11
```
