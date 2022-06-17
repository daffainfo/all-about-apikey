# [ScrapingDog](https://www.scrapingdog.com/documentation)

## __Description__
Proxy API for Web scraping

## __Example Request__
* Curl
```
curl "https://api.scrapingdog.com/scrape?api_key={{token}}&url=https://example.com/ip&dynamic=false"
```

* Raw
```
GET /scrape?api_key={{token}}&url=https://example.com/ip&dynamic=false HTTP/1.1
Host: api.scrapingdog.com
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
    "message":"Unauthorized request, please make sure your API key is valid.",
    "success":false
}
```
## __Regex__
```
[a-z0-9]{24}
```

## __Example API key__
```
5e5a97e5b1ca5b194f42da86
```
