# [ReviewApi](https://app.reviewapi.io/documentation)

## __Description__
Review API to scrape structured and normalized JSON review data from 10+ review platforms to build your apps or custom reports.

## __Example Request__
* Curl
```
curl "https://app.reviewapi.io/api/v1/reviews?apikey={{token}}&url=https%3A%2F%2Fwww.capterra.com%2Fp%2F140650%2FRecruitee%2Freviews&amount=25"
```

* Raw
```
GET /api/v1/reviews?apikey={{token}}&url=https%3A%2F%2Fwww.capterra.com%2Fp%2F140650%2FRecruitee%2Freviews&amount=25 HTTP/1.1
Host: app.reviewapi.io
...
```

## __Response__
* Success
```
{
    "id": "kzPdyP7bQr",
    "state": "queued",
    "url": "https://reviewapi.lan/api/v1/batches/kzPdyP7bQr", 
    "jobs": [
       "kQBeXDWeyK"
    ]
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