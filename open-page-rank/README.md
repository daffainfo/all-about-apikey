# [Open Page Rank](https://www.domcop.com/openpagerank/documentation)

## __Description__
API for calculating and comparing metrics of different websites using Page Rank algorithm

## __Example Request__
* Curl
```
curl "https://openpagerank.com/api/v1.0/getPageRank?domains[]=google.com" -H "API-OPR: {{token}}"
```

* Raw
```
GET /api/v1.0/getPageRank?domains[]=google.com HTTP/1.1
Host: openpagerank.com
API-OPR: {{token}}
```

## __Response__
* Success
```
{
    "status_code":200,
    "response":[
        {
            "status_code":200,
            "error":"",
            "page_rank_integer":10,
            "page_rank_decimal":10,
            "rank":"3",
            "domain":"google.com"
        }
    ],
    "last_updated":"19th Mar 2022"
}
```
* Error
```
{
    "status":false,
    "error":"Invalid API key "
}
```
## __Regex__
```
[gcswkso048]{40}
```

## __Example API key__
```
cwkg044cggswwo0c8wcw80cok4o40g0o48s0go48
```
