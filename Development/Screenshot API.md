# [Screenshot API](https://docs.screenshotapi.net/?ref=webflow)

## __Description__
Create pixel-perfect website screenshots

## __Example Request__
* Curl
```
curl "https://shot.screenshotapi.net/screenshot?token={{token}}&url=https://example.com"
```

* Raw
```
GET /screenshot?token={{token}}&url=https://example.com HTTP/1.1
Host: shot.screenshotapi.net
```

## __Response__
* Success
```
{
    "screenshot":"https://screenshoapi.....",
    "url":"https://example.com",
    "created_at":"2022-06-17T16:06:29.435Z",
    "is_fresh":true,
    "token":"{{token}}",
    "ttl":"2022-07-17T16:06:25.255Z"
}
```
* Error
```
{
    "error":"Unuathorized 2"
}
```
## __Regex__
```
[A-Z0-9]{7}-[A-Z0-9]{7}-[A-Z0-9]{7}-[A-Z0-9]{7}
```

## __Example API key__
```
03S7N6P-VDGM7JT-Q6F7XQW-31K8Q32
```
