# [Google Books](https://developers.google.com/books/docs/overview)

## __Description__
Google Books

## __Example Request__
* Curl
```
curl "https://www.googleapis.com/books/v1/volumes/zyTCAlFPjgYC?key={{token}}"
```

* Raw
```
GET /books/v1/volumes/zyTCAlFPjgYC?key={{token}} HTTP/1.1
Host: www.googleapis.com
```

## __Response__
* Success
```
{
    "error": {
        "code": 400,
        "message": "API key not valid. Please pass a valid API key.",
        "errors": [
            {
            "message": "API key not valid. Please pass a valid API key.",
            "domain": "global",
            "reason": "badRequest"
            }
        ],
        "status": "INVALID_ARGUMENT"
    }
}
```
* Error
```
{
    "kind": "books#volume",
    "id": "zyTCAlFPjgYC",
    "etag": "f0zKg75Mx/I",
    "selfLink": "https://www.googleapis.com/books/v1/volumes/zyTCAlFPjgYC",
    "volumeInfo": {
        "title": "The Google story",
        "authors": [
            "David A. Vise",
            "Mark Malseed"
        ],
    ...
```

## __Regex__
```
AIza[0-9A-Za-z-_]{35}
```

## __Example API key__
```
AIzaSyAtUXpd8JxrpUH2Sd-xO2U_vWGVfoF5-XM
```