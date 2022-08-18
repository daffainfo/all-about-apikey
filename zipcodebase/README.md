# [Zipcodebase](https://app.zipcodebase.com/documentation)

## __Description__
Lookup postal codes, calculate distances and much more with our free zip code api.

## __Example Request__
* Curl
```
curl "https://app.zipcodebase.com/api/v1/search?apikey={{token}}&codes=10005%2C51503"
```

* Raw
```
GET /api/v1/search?apikey={{token}}&codes=10005%2C51503 HTTP/1.1
Host: app.zipcodebase.com
...
```

## __Response__
* Success
```
{
   "query":{
      "codes":[
         "10005",
         "51503"
      ],
      "country":null
   },
   "results":{
      "10005":[
         {
            "postal_code":"10005",
            "country_code":"DZ",
            "latitude":"36.26960000",
            "longitude":"3.66360000",
            "city":"Ouled Zidane",
            "state":"Bouira",
            "state_code":"10",
            "province":null,
            ...
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