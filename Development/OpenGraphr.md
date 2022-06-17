# [OpenGraphr](https://opengraphr.com/docs/1.0/overview)

## __Description__
Really simple API to retrieve Open Graph data from an URL

## __Example Request__
* Curl
```
curl "https://api.opengraphr.com/v1/og?api_token={{token}}&url=https://google.com"
```

* Raw
```
GET /v1/og?api_token={{token}}&url=https://google.com HTTP/1.1
Host: api.opengraphr.com
```

## __Response__
* Success
```
{
    "title":"Google",
    "image":"https://www.google.com/logos/doodles/2022/celebrating-amanda-aldridge-6753651837109368-l.png",
    "url":"https://google.com",
    "reading_time_in_minutes":2,
    "raw":{
        "title":"Google"
    },
    "validUntil":1658066063236
}
```
* Error
```
{
    "error":"Could not verify token"
}
```
## __Regex__
```
[a-zA-Z0-9]{80}
```

## __Example API key__
```
f0eyBlspFIwoXZbI60aqf0eyBlspFIwoXZbI60aqf0eyBlspFIwoXZbI60aqf0eyBlspFIwoXZbI60aq
```
