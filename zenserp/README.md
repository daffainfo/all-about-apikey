# [Zenserp](https://app.zenserp.com/documentation)

## __Description__
Scrape search engine result pages in realtime

## __Example Request__
* Curl
```
curl "https://app.zenserp.com/api/v2/status?apikey={{token}}"
```

* Raw
```
GET /api/v2/status?apikey={{token}} HTTP/1.1
Host: app.zenserp.com
...
```

## __Response__
* Success
```
{
    "remaining_requests": 1500
}
```
* Error
```
{
    "error":"Not enough requests."
}
```

## __Regex__
```
[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}
```

## __Example API key__
```
da3ec69e-bdc3-8f07-b5e3-6521c026d4be
```