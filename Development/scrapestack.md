# [scrapestack](https://scrapestack.com/documentation)

## __Description__
Real-time, Scalable Proxy & Web Scraping REST API

## __Example Request__
* Curl
```
curl "https://api.scrapestack.com/scrape?access_key={{token}}&url=https://example.com"
```

* Raw
```
GET /scrape?access_key={{token}}&url=https://example.com HTTP/1.1
Host: api.scrapestack.com
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
    "success":false,
    "error":{
        "code":101,
        "type":"invalid_access_key",
        "info":"You have not supplied a valid API Access Key. [Technical Support: support@apilayer.com]"
    }
}
```
## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
tue3sv9hzsey1me4l7fwq3t46u5k8wag
```
