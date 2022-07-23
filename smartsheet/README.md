# [Smartsheet](https://smartsheet.redoc.ly/)

## __Description__
Allows you to programmatically access and Smartsheet data and account information

## __Example Request__
* Curl
```
curl 'https://api.smartsheet.com/2.0/home?include=source' -H "Authorization: Bearer {{token}}"
```

* Raw
```
GET /2.0/home?include=source HTTP/1.1
Authorization: Bearer {{token}}
Host: api.smartsheet.com
```

## __Response__
* Success
```
{
    "sheets":[],
    "folders":[],
    "workspaces":[]
}
```
* Error
```
{
  "errorCode" : 1002,
  "message" : "Your Access Token is invalid.",
  "refId" : "xxxxxxxxxxxx"
}
```

## __Regex__
```
[a-z0-9]{26}
```

## __Example API key__
```
bb1aa18d0eeea0fc7ggg799h3i
```