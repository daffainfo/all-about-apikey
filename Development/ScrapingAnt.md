# [ScrapingAnt](https://docs.scrapingant.com/)

## __Description__
Headless Chrome scraping with a simple API	

## __Example Request__
* Curl
```
curl --request POST --url "https://api.scrapingant.com/v1/general" --header "x-api-key: {{token}}" --header "accept: application/json" --header "content-type: application/json" --data '{"url": "https://example.com"}'
```

* Raw
```
POST /v1/general HTTP/1.1
Host: api.scrapingant.com
x-api-key: {{token}}
Accept: application/json
Content-Type: application/json]

{"url": "https://example.com"}
```

## __Response__
* Success
```
{
    "content": "<!DOCTYPE html><html><head>\n    <title>Example Domain</title>\n\n    <meta charset=\"utf-8\">\n    <meta http-equiv=\"Content-type\" content=\"text/html; charset=utf-8\">\n    <meta name=\"viewport\" content=\"width=device-width, initial-scale=1\">\n    <style type=\"text/css\">\n    body {\n        background-color: #f0f0f2;\n        margin: 0;\n        padding: 0;\n        font-family: -apple-system, system-ui, BlinkMacSystemFont, \"Segoe UI\", \"Open Sans\", \"Helvetica Neue\", Helvetica, Arial, sans-serif;\n        \n    }\n    div {\n        width: 600px;\n        margin: 5em auto;\n        padding: 2em;\n        background-color: #fdfdff;\n        border-radius: 0.5em;\n        box-shadow: 2px 3px 7px 2px rgba(0,0,0,0.02);\n    }\n    a:link, a:visited {\n        color: #38488f;\n        text-decoration: none;\n    }\n    @media (max-width: 700px) {\n        div {\n            margin: 0 auto;\n            width: auto;\n        }\n    }\n    </style>    \n</head>\n\n<body>\n<div>\n    <h1>Example Domain</h1>\n    <p>This domain is for use in illustrative examples in documents. You may use this\n    domain in literature without prior coordination or asking for permission.</p>\n    <p><a href=\"https://www.iana.org/domains/example\">More information...</a></p>\n</div>\n\n\n</body></html>",
    "cookies": "",
    "status_code": 200
}
```
* Error
```
{
    "detail": "API token is wrong. Please visit https://app.scrapingant.com/profile to check your token settings"
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