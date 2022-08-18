# [SportdataAPI](https://app.sportdataapi.com/documentation)

## __Description__
Get sports data from all over the world with our sports data API

## __Example Request__
* Curl
```
curl "https://app.sportdataapi.com/api/v1/soccer/countries?apikey={{token}}&continent=Europe"
```

* Raw
```
GET /api/v1/soccer/countries?apikey={{token}}&continent=Europe HTTP/1.1
Host: app.sportdataapi.com
...
```

## __Response__
* Success
```
{
   "query":{
      "continent":"Europe"
   },
   "results":[
        {
            "id":135,
            "name":"Europe",
            "country_code":null,
            "continent":"Europe"
        },
        {
            "id":8,
            "name":"Albania",
            "country_code":"al",
            "continent":"Europe"
        },
        ...
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