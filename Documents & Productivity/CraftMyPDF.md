# [CraftMyPDF](https://pdflayer.com/documentation)

## __Description__
Generate PDF documents from templates with a drop-and-drop editor and a simple API

## __Example Request__
* Curl
```
curl --header "Content-Type: application/json"  \
      --header 'X-API-KEY: {{token}}' \
      "https://api.craftmypdf.com/v1/list-templates?limit=300&offset=0"
```

* Raw
```
GET /v1/list-templates?limit=300&offset=0 HTTP/1.1
Host: api.craftmypdf.com
Content-Type: application/json
X-API-KEY: {{token}}
```

## __Response__
* Success
```
{
    "status": "success",
    "templates": [
        {
            "template_id": "5ef77b2b187c968c",
            "name": "Invoice Template",
            "status": "ACTIVE",
            "created_at": "2021-07-31T16:00:00.000Z",
            "updated_at": "2021-08-27T13:07:45.968Z",
            "group_name": ""
        },
        {
            "template_id": "19d77b2b187554e0",
            "name": "PDF Template",
            "status": "ACTIVE",
            "created_at": "2020-06-31T16:00:00.000Z",
            "updated_at": "2021-08-27T13:07:45.968Z",
            "group_name": ""
        }
    ]
}
```
* Error
```
{
    "status":"error",
    "message":"Invalid API Key"
}
```
## __Regex__
```
[a-zA-Z0-9]{35}
```

## __Example API key__
```
tue3sv9hzsey1me4l7fwq3t46u5k8wagavd
```
