# [JSONBin](https://jsonbin.io/api-reference)

## __Description__
Free JSON storage service. Ideal for small scale Web apps, Websites and Mobile apps

## __Example Request__
* Curl
```
curl "https://api.jsonbin.io/v3/c" -H "X-Master-key: {{token}}"
```

* Raw
```
GET /v3/c HTTP/1.1
Host: api.jsonbin.io
X-Master-key: {{token}}
```

## __Response__
* Success
```
[
    {
        "record": "<COLLECTION_ID>",
        "collectionMeta": {
            "name": "<COLLECTION_NAME>"
        },
        "schemaDocId": "<SCHEMA_DOC_ID>"
        "createdAt": "<DATE_TIME>"
    }
    ...
]
```
* Error
```
{
    "message":"Invalid X-Master-Key provided"
}
```
## __Regex__
```
\$2b\$10\$[a-zA-Z0-9\/]{53}
```

## __Example API key__
```
$2b$10$TSBN31bgq1btrJOM0i1r0e3631W/AvASXKBqyV9Hra/1sAoehKAAe
```
