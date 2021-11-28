# [Instatus](https://instatus.com/help/api)

## __Description__
Post to and update maintenance and incidents on your status page through an HTTP REST API

## __Example Request__
* Curl
```
curl -H "Authorization: Bearer {{token}}" https://api.instatus.com/v1/pages
```

* Raw
```
GET /v1/pages HTTP/1.1
Authorization: Bearer {{token}}
Host: api.instatus.com
```

## __Response__
* Success
```
[
    {
        "id":"xxxxxxxxxxxxxxx",
        "subdomain":"test",
        "name":"test",
        "logoUrl":null,
        "faviconUrl":null,
        "websiteUrl":null,
        "customDomain":null,
        "publicEmail":null,
        "twitter":null,
        "status":"UP",
        "subscribeBySms":false,
        "sendSmsNotifications":true,
        ...
    }
]
```
* Error
```
{
    "error":{
        "code":"forbidden",
        "message":"API key does not belong to a user."
    }
}
```

## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
bb1aa18d0eeea0fc7ggg799h3i9578j
```