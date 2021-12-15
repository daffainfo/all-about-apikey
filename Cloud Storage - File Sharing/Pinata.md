# [Pinata](https://docs.pinata.cloud/)

## __Description__
IPFS Pinning Services API

## __Example Request__
* Curl
```
curl "https://api.pinata.cloud/data/pinList?status=pinned" -H "pinata_api_key:4ce3a7d51ec746ec3580" -H "pinata_secret_api_key: fdeadcdb93970485af97f6ef62ee177ea632a24f4c6bb81a77c218cfc0dba87d"
```

* Raw
```
GET /data/pinList?status=pinned HTTP/1.1
Host: api.pinata.cloud
pinata_api_key: {{api_key}}
pinata_secret_api_key: {{secret_api_key}}
```

## __Response__
* Success

```
{
    "count":1151,
    "rows":[
        {
            "id":"xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
            "ipfs_pin_hash":"xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
            "size":11111,
            "user_id":"xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
            "date_pinned":"2021-11-08T14:59:16.410Z",
            "date_unpinned":null,
            "metadata"
            ...
        }
    ]
}
```
* Error
```
{
    "error":{
        "reason":"KEYS_MUST_BE_STRINGS",
        "details":"pinata_api_key and pinata_secret_api_key must both be strings"
    }
}
```

## __Regex__
* API Key
```
[a-z0-9]{20}
```
* Secret API Key
```
[a-z0-9]{64}
```

## __Example key__
* API Key
```
4le3a2gc3aa333aa3c31
```
* Secret API Key
```
4le3a2gc3aa333aa3c314le3a2gc3aa333aa3c314le3a2gc3aa333aa3c311234
```