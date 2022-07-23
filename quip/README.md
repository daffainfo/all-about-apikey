# [Quip](https://quip.com/dev/automation/documentation)

## __Description__
File Sharing and Storage for groups

## __Example Request__
* Curl
```
curl "https://platform.quip.com/1/users/contacts" -H "Authorization: Bearer {{token}}"
```

* Raw
```
GET /1/users/contacts HTTP/1.1
Host: platform.quip.com
Authorization: Bearer {{token}}
```

## __Response__
* Success
```
[]
```
* Error
```
{
    "error":"application_error",
    "error_code":401,
    "error_description":"Invalid access_token"
}
```

## __Regex__
```
[a-zA-Z0-9]{15}=\|[0-9]{10}\|[a-zA-Z0-9\/+]{43}=
```

## __Example API key__
```
RFlRQU1BU2RNN20=|1668953676|OZni5d8LGfRkgIcW8YgVY/wyhHhoUaSRncJK+QF6W0k=
```