# [ProxyCrawl](https://proxycrawl.com/docs/)

## __Description__
Scraping and crawling anticaptcha service

## __Example Request__
* Curl
```
curl "https://api.proxycrawl.com/leads?token={{token}}&domain=www.amazon.com"
```

* Raw
```
GET /leads?token={{token}}&domain=www.amazon.com HTTP/1.1
Host: api.proxycrawl.com
```

## __Response__
* Success
```
{
    "success": true,
    "remaining_requests": 100,
    "domain": "www.amazon.com",
    "leads": [
        ...
    ]
}
```
* Error
```
{
    "pc_status":403,
    "error":"Token is invalid or account is temporarily blocked! please login to your dashboard for more details"
}
```
## __Regex__
```
[a-zA-Z0-9_]{22}
```

## __Example API key__
```
kuEkyhxkL2ckwS_YG8nyRg
```
