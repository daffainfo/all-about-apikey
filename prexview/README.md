# [PrexView](https://prexview.com/docs)

## __Description__
Data from XML or JSON to PDF, HTML or Image

## __Example Request__
* Curl
```
curl -H "Authorization: {{token}}" \
  https://api.prexview.com/v1/transform \
  -F json="{\"hello\":\"World\"}" \
  -F template="template-name" \
  -F output="pdf" \
  -o result.pdf
```

* Raw
```
POST /v1/transform HTTP/1.1
Host: api.prexview.com
Authorization: {{token}}
Content-Type: multipart/form-data; boundary=---abcd1234abcd1234abcd

---abcd1234abcd1234abcd
Content-Disposition: form-data; name="json"

{\"hello\":\"World\"}
---abcd1234abcd1234abcd
Content-Disposition: form-data; name="template"

template-name
---abcd1234abcd1234abcd
Content-Disposition: form-data; name="output"

pdf
---abcd1234abcd1234abcd--
```

## __Response__
* Success
```
Automatically download pdf
```
* Error
```
{
    "error":{
        "name":"Error",
        "status":401,
        "message":"Authorization Required",
        "statusCode":401,
        "code":"AUTHORIZATION_REQUIRED"
    }
}
```

## __Regex__
```
[a-zA-Z0-9]{64}
```

## __Example API key__
```
BZyM5NrOFggEKScKxgXksF3nRHxTaJS8omSqcrE2oa7x7RekATlVYeJZ9BZGUrQd
```