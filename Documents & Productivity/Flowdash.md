# [Flowdash](https://docs.flowdash.com/docs/api-introduction)

## __Description__
Automate business workflows

## __Example Request__
* Curl
```
curl https://app.flowdash.com/api/v1/workflows --header "Authorization: Bearer {{token}}"
```

* Raw
```
GET /api/v1/workflows HTTP/1.1
Host: app.flowdash.com
Authorization: Bearer {{token}}
```

## __Response__
* Success
```
[
    {
        "id":"12DK2q",
        "name":"Testing 1"
    },
    {
        "id":"12DK2q",
        "name":"Testing 2"
    }
]
```
* Error
```
401 Unauthorized
```
## __Regex__
```
[a-zA-Z0-9]{24}
```

## __Example API key__
```
tue3sv9hzsey1me4l7fwq3t4
```
