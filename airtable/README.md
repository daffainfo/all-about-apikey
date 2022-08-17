# [Airtable](https://airtable.com/api)

## __Description__
Integrate with Airtable

## __Example Request__
* Curl
```
curl "https://api.airtable.com/v0/meta/bases" -H "Authorization: Bearer {{token}}"
```

* Raw
```
GET /v0/meta/bases HTTP/1.1
Host: api.airtable.com
Authorization: Bearer {{token}}
```

## __Response__
* Success
```
{
    "bases": [
        {
            "id": "appY3WxIBCdKPDdIa",
            "name": "Apartment Hunting",
            "permissionLevel": "create"
        },
        {
            "id": "appSW9R5uCNmRmfl6",
            "name": "Project Tracker",
            "permissionLevel": "edit"
        }
    ]
}
```
* Error
```
{
    "error":{
        "type":"UNAUTHORIZED",
        "message":"Invalid authentication token"
    }
}
```
## __Regex__
```
key[a-zA-Z0-9]{14}
```

## __Example API key__
```
key3jaF0r7yhRPZDU
```
