# [GoFile](https://gofile.io/api)

## __Description__
Unlimited size file uploads for free

## __Example Request__
* Curl
```
curl "https://api.gofile.io/getAccountDetails?token={{token}}&allDetails=true"
```

* Raw
```
GET /getAccountDetails?token={{token}}&allDetails=true HTTP/1.1
Host: api.gofile.io
```

## __Response__
* Success
```
{
    "status":"ok",
    "data":{
        "token":"{{token}}",
        "email":"example@gmail.com",
        "tier":"standard",
        "rootFolder":"xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
        "filesCount":0,
        "filesCountLimit":null,
        "totalSize":0,
        "totalSizeLimit":null,
        "total30DDLTraffic":0,
        "total30DDLTrafficLimit":null
    }
}
```
* Error
```
{
    "status":"error-wrongToken",
    "data":{}
}
```

## __Regex__
```
[a-zA-Z0-9]{32}
```

## __Example API key__
```
OF3ab02f3cD12lDOfxc3foSg129sD241
```