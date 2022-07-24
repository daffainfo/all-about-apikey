# [Abstract Company Enrichment](https://www.abstractapi.com/api/company-enrichment)

## __Description__
Enrich any domain or email with accurate company data, including headcount, location and industry.

## __Example Request__
* Curl
```
curl "https://companyenrichment.abstractapi.com/v1/?api_key={{token}}&domain=airbnb.com"
```

* Raw
```
GET /v1/?api_key={{token}}&domain=airbnb.com HTTP/1.1
Host: companyenrichment.abstractapi.com
```

## __Response__
* Success
```
{
    "name": "Airbnb",
    "domain": "airbnb.com",
    "year_founded": 2008,
    "industry": "Internet",
    "employees_count": 14604,
    "locality": "San Francisco",
    "country": "United States",
    "linkedin_url": "linkedin.com/company/airbnb"
}
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