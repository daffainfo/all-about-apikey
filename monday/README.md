# [Monday](https://api.developer.monday.com/docs)

## __Description__
Programmatically access and update data inside a monday.com account

## __Example Request__
* Curl
```
curl --location --request POST 'https://api.monday.com/v2' \
    --header 'Authorization: {{token}}' \
    --header 'Content-Type: application/json' \
    --data-raw '{"query": "query { me { is_guest created_at name id}}"}'
```

* Raw
```
POST /v2 HTTP/1.1
Host: api.monday.com
Authorization: {{token}}
Content-Type: application/json
Content-Length: 55

{"query": "query { me { is_guest created_at name id}}"}
```

## __Response__
* Success
```
{
    "data": {
        "me": {
        "is_guest": false,
        "created_at": "2022-07-22T07:02:26Z",
        "name": "Test Test",
        "id": 123456789
        }
    },
    "account_id": 12345678
}
```
* Error
```
{
    "errors": ["Not Authenticated"]
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