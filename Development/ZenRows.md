# [ZenRows](https://www.zenrows.com/documentation/)

## __Description__
Web Scraping API that bypasses anti-bot solutions while offering JS rendering, and rotating proxies

## __Example Request__
* Curl
```
curl "https://api.zenrows.com/v1/?apikey={{token}}&url=https://example.com"
```

* Raw
```
GET /v1/?apikey={{token}}&url=https://example.com HTTP/1.1
Host: api.zenrows.com
```

## __Response__
* Success
```
<!doctype html>
<html>
<head>
    <title>Example Domain</title>

    <meta charset="utf-8" />
    <meta http-equiv="Content-type" content="text/html; charset=utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <style type="text/css">
    body {
        background-color: #f0f0f2;
        margin: 0;
        padding: 0;
        font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI", "Open Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;

    }
    ...
```
* Error
```
{
    "error":1,
    "error_message":"invalid APIkey provided"
}
```
## __Regex__
```
[a-z0-9]{40}
```

## __Example API key__
```
2f418a732f418a732f418a732f418a732f418a73
```
