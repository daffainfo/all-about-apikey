# [SearchApi](https://www.searchapi.io/docs/google)

## Description
Real-time Google SERP API

## __Example Request__
* Curl
```
curl "https://www.searchapi.io/api/v1/search?api_key={{token}}&engine=google&q=AI"
```

* Raw
```
GET /api/v1/search?api_key={{token}}&engine=google&q=chatgpt HTTP/1.1
Host: www.searchapi.io
```

## __Response__
* Success
```
{
  "search_metadata": {
    "id": "search_zx6dAL2p4KqYsxVxk7wnGOmN",
    "status": "Success",
    "created_at": "2023-08-14T11:09:36Z",
    "request_time_taken": 1.03,
    "parsing_time_taken": 0.15,
    "total_time_taken": 1.19,
    "request_url": "https://www.google.com/search?q=AI&oq=AI&gl=us&hl=en&ie=UTF-8",
    "html_url": "https://www.searchapi.io/api/v1/searches/search_zx6dAL2p4KqYsxVxk7wnGOmN.html",
    "json_url": "https://www.searchapi.io/api/v1/searches/search_zx6dAL2p4KqYsxVxk7wnGOmN"
  },
  "search_parameters": {
    "engine": "google",
    "q": "AI",
    "device": "desktop",
    "google_domain": "google.com",
    "hl": "en",
    "gl": "us"
  },
  ...
}
```
* Error
```
{
  "error": "Invalid API key."
}
```

## __Regex__
```
[a-f0-9]{32}
```

## __Example API key__
```
57c3219371de68c9128b6788488a0ef3
```
