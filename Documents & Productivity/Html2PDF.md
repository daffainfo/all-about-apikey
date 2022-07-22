# [Html2PDF](https://html2pdf.app/documentation/)

## __Description__
HTML/URL to PDF

## __Example Request__
* Curl
```
curl "https://api.html2pdf.app/v1/generate?url=https://example.com&apiKey={{token}}"
```

* Raw
```
GET /v1/generate?url=https://example.com&apiKey={{token}} HTTP/1.1
Host: api.html2pdf.app
```

## __Response__
* Success
```
Will download PDF file of example.com
```
* Error
```
{
    "errorCode":6,
    "message":"Unauthorized"
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
