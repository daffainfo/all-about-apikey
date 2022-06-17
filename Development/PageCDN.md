# [PageCDN](https://pagecdn.com/docs/public-api)

## __Description__
Public API for javascript, css and font libraries on PageCDN

## __Example Request__
* Curl
```
curl "https://pagecdn.com/api/v2/private/repo/files?apikey={{token}}&repo=site/wxyz"
```

* Raw
```
GET /api/v2/private/repo/files?apikey={{token}}&repo=site/wxyz HTTP/1.1
Host: pagecdn.com
```

## __Response__
* Success
```
{
    "status": "200",
    "message": "Ok",
    "details": "Success",
    "response": {
        "count": 5282,
        "files": [
            {
                "version": "3.4.0",
                "file_hash": "0d864c082f074c2f900ebe5035a21c7d1ed548fb5c212ca477ee9e4a6056e6aa",
                "file_url": "https://pagecdn.io/repo/wxyz/3.4.0/scripts.js"
            },
            ...
```
* Error
```
{
    "status": "401",
    "message": "Unauthorized",
    "details": "Invalid API Key.",
    "response": []
}
```
## __Regex__
```
[a-z0-9]{64}
```

## __Example API key__
```
wrion7bk4lh7pxp2wiq57mjak6s0tp34fj1fiemdjqj1g5xl57hi3km8g6jpv28z
```
