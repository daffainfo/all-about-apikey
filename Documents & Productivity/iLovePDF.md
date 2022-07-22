# [iLovePDF](https://developer.ilovepdf.com/docs/api-reference)

## __Description__
Convert, merge, split, extract text and add page numbers for PDFs. Free for 250 documents/month	

## __Example Request__
* Curl
```
curl "https://api.pdflayer.com/api/convert?access_key={{token}}&document_url=https://pdflayer.com/downloads/invoice.html"
```

* Raw
```
GET /api/convert?access_key={{token}}&document_url=https://pdflayer.com/downloads/invoice.html HTTP/1.1
Host: api.pdflayer.com
...
```

## __Response__
* Success
```
Automatically download pdf
```
* Error
```
{
    "success":false,
    "error": {
        "code":101,
        "type":"invalid_access_key",
        "info":"You have not supplied a valid API Access Key. [Technical Support: support@apilayer.com]"
    }
}
```
## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
tue3sv9hzsey1me4l7fwq3t46u5k8wag
```
