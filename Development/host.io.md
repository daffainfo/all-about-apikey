# [host.io](https://host.io/docs)

## __Description__
Domains Data API for Developers

## __Example Request__
* Curl
```
curl "https://host.io/api/full/facebook.com?token=${{token}}"
```

* Raw
```
GET /api/full/facebook.com?token=${{token}} HTTP/1.1
Host: host.io
```

## __Response__
* Success
```
{
    "domain": "facebook.com",
    "web": {
        "domain": "facebook.com",
        "rank": 3,
        "url": "https://m.facebook.com/?_rdr",
        "ip": "157.240.11.35",
        "date": "2022-05-25T20:35:10.915Z",
        "length": 59649,
        "encoding": "utf8",
        "copyright": "Meta Â© 2022",
        "facebook": "images",
        "title": "Facebook - log in or sign up",
        ...
```
* Error
```
{
    "error": "Please ensure you've entered your token correctly.",
    "title": "Unknown Token"
}
```
## __Regex__
```
[a-z0-9]{14}
```

## __Example API key__
```
kj5c23a1d263d9
```
