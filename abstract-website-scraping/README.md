# [Abstract Web Scraping](https://www.abstractapi.com/api/web-scraping-api)

## __Description__
Scrape and extract data from any website, with powerful options like proxy / browser customization, CAPTCHA handling, ad blocking, and more.

## __Example Request__
* Curl
```
curl "https://scrape.abstractapi.com/v1/?api_key={{token}}&url=https://www.apple.com"
```

* Raw
```
GET /v1/?api_key={{token}}&url=https://www.apple.com HTTP/1.1
Host: scrape.abstractapi.com
```

## __Response__
* Success
```
<!DOCTYPE html>

<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en-US" lang="en-US">'

    <head>
       [...] // 46 lines skipped
    </head>
   
    <body>
       [...] // 512 lines skipped
    </body>

</html>
```
* Error
```
{
    "error":{
        "message":"Invalid API key provided.",
        "code":"unauthorized",
        "details":null
    }
}
```

## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
of3ab02f3xd12ldofxc3fosc129sd241
```