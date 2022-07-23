# [Micro User Service](https://m3o.com/user)

## __Description__
User management and authentication

## __Example Request__
* Curl
```
curl "https://api.m3o.com/v1/user/Read" \
-H "Content-Type: application/json" \
-H "Authorization: Bearer {{token}}" \
-d '{
  "id": "usrid-1"
}'
```

* Raw
```
POST /v1/user/Read HTTP/1.1
Host: api.m3o.com
Content-Type: application/json
Authorization: Bearer {{token}}
Content-Length: 21

{
  "id": "usrid-1"
}
```

## __Response__
* Success
```
{
    "account": {
        "id": "fdf34f34f34-f34f34-f43f43f34-f4f34f",
        "username": "usrname-1",
        "email": "joe@example.com",
        "created": "1623677579",
        "updated": "1623677579"
    }
}
```
* Error
```
{
    "Id":"v1",
    "Code":401,
    "Detail":"Unauthorized",
    "Status":"Unauthorized"
}
```

## __Regex__
```
[A-Za-z0-9]{48}
```

## __Example API key__
```
YQ6wba4vACaht9CUK9k5N7QxV2ieRPJ396g94vkWSYauYmch
```
