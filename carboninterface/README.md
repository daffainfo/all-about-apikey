# [Carbon Interface](https://docs.carboninterface.com/#/)

## __Description__
API to calculate carbon (C02) emissions estimates for common C02 emitting activities

## __Example Request__
* Curl
```
curl "https://www.carboninterface.com/api/v1/auth" -H "Authorization: Bearer {{token}}"
```

* Raw
```
GET /api/v1/auth HTTP/1.1
Host: www.carboninterface.com
Authorization: Bearer {{token}}
```

## __Response__
* Success
```
{
    "message":"auth successful"
}
```
* Error
```
HTTP Token: Access denied.
```
## __Regex__
```
[a-zA-Z0-9]{21}
```

## __Example API key__
```
oDWwEm2KepcmbsLbCK2ld
```