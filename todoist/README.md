# [Todoist](https://developer.todoist.com/rest/v1/#overview)

## __Description__
Todo Lists

## __Example Request__
* Curl
```
curl "https://api.todoist.com/rest/v1/projects" -H "Authorization: Bearer {{token}}"
```

* Raw
```
GET /rest/v1/projects HTTP/1.1
Host: api.todoist.com
Authorization: Bearer {{token}}
```

## __Response__
* Success
```
[
    {
        "id": 123456789,
        "color": 11,
        "name": "Inbox",
        "comment_count": 0,
        "shared": false,
        "favorite": false,
        "sync_id": 0,
        "inbox_project": true,
        "url": "https://todoist.com/showProject?id=123456789"
    },
    ...
]
```
* Error
```
Forbidden
```

## __Regex__
```
[a-z0-9]{40}
```

## __Example API key__
```
tue3sv9hzsey1me4l7fwq3t46u5k8wagabcdefgh
```