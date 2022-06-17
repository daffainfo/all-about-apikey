# [Gorest](https://gorest.co.in/)

## __Description__
Online REST API for Testing and Prototyping

## __Example Request__
* Curl
```
curl -H "Accept:application/json" -H "Content-Type:application/json" -H "Authorization: Bearer {{token}}" -XDELETE "https://gorest.co.in/public/v2/users/5"
```

* Raw
```
GET /public/v2/users/5 HTTP/1.1
Host: gorest.co.in
Accept: application/json
Content-Type: application/json
Authorization: Bearer {{token}}
```

## __Response__
* Success

the response doesn't have body and the status code is `204`

* Error
```
{
    "message":"Resource not found"
}
```
## __Regex__
```
[a-z0-9]{65}
```

## __Example API key__
```
7ee098783b36b76b471bd47bee1ff16e1f63db2267fc105c145daa7cca5981580
```
