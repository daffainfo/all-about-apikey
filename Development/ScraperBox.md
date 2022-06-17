# [ScraperBox](https://scraperbox.com/documentation)

## __Description__
Undetectable web scraping API

## __Example Request__
* Curl
```
curl "https://api.scraperbox.com/scrape?token={{token}}&url=https://example.com"
```

* Raw
```
GET /scrape?token={{token}}&url=https://example.com HTTP/1.1
Host: api.scraperbox.com
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
    "errors":{
        "token":"Invalid API token provided."
    }
}
```
## __Regex__
```
[A-Z0-9]{32}
```

## __Example API key__
```
371328EEA9E093B8371328EEA9E093B8
```
