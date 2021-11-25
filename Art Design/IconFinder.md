# [IconFinder](https://developer.iconfinder.com/reference/overview-1)

## __Description__
Web Icons

## __Example Request__
* Curl
```
curl --request GET \
     --url "https://api.iconfinder.com/v4/icons/search?query=arrow&count=10" \
     --header "Accept: application/json" \
     --header "Authorization: Bearer {{token}}"
```

* Raw
```
GET /v4/icons/search?query=arrow&count=10 HTTP/1.1
Host: api.iconfinder.com
Accept: application/json
Authorization: Bearer {{token}}
```

## __Response__
* Success
```
{
    "total_count": 108035,
    "icons": [
    {
        "categories": [
        {
            "name": "UI",
            "identifier": "ui"
        }
    ],
    "containers": [
        {
            "format": "ico",
            "download_url": "https://api.iconfinder.com/v4/icons/389801/containers/ico/download"
        },
    ...
```
* Error
```
{}
```

## __Regex__
```
[a-zA-Z0-9]{64}
```

## __Example API key__
```
BZyM5NrOFggEKScKxgXksF3nRHxTaJS8omSqcrE2oa7x7RekATlVYeJZ9BZGUrQd
```
