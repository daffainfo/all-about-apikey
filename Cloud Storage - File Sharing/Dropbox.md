# [Dropbox](https://www.dropbox.com/developers)

## __Description__
File Sharing and Storage

## __Example Request__
* Curl
```
curl -X POST https://api.dropboxapi.com/2/check/user \
  --header 'Authorization: Bearer {{token}}' \
  --header 'Content-Type: application/json' \
  --data '{}'
```

* Raw
```
POST /2/check/user HTTP/1.1
Host: api.dropboxapi.com
Authorization: Bearer {{token}}
Content-Type: application/json
Content-Length: 2

{}
```

## __Response__
* Success
```
{
  "result": ""
}
```
* Error
```
{
  "error": {
    ".tag": "invalid_access_token"
  },
  "error_summary": "invalid_access_token/"
}
```

## __Regex__
```
sl.[a-zA-Z0-9_-]{136}
```

## __Example API key__
```
sl.ONOIUgObmbrgsga1kBI-q4NrS_R2cplbTe6zF9ImkQbiR7reMEke4Pcc_hhDtj7uGeEwGB5RmDKQrYclvhvQOkcPBWHRtkBqVabX5_gEhM-y_ZkXDtTQmUrK8gVq8j8YIIl9w8_B
```