# [Web3 Storage](https://docs.web3.storage/)

## __Description__
File Sharing and Storage for Free with 1TB Space

## __Example Request__
* Curl
```
curl "https://api.web3.storage/user/uploads" -H "Authorization: Bearer {{token}}"
```

* Raw
```
GET /user/uploads HTTP/1.1
Host: api.web3.storage
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
    "code":"ERROR_TOKEN_NOT_FOUND",
    "message":"API token no longer valid"
}
```
or
```
{
    "code":"ERROR_UNRECOGNISED_TOKEN",
    "message":"Could not parse provided API token"
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