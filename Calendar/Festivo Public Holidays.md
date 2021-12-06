# [Festivo Public Holidays](https://docs.getfestivo.com/docs/products/public-holidays-api/intro)

## __Description__
Fastest and most advanced public holiday and observance service on the market

## __Example Request__
* Curl
```
curl "https://api.getfestivo.com/v2/holidays?country=US&api_key={{token}}&year=2020"
```

* Raw
```
GET /v2/holidays?country=US&api_key={{token}}&year=2020 HTTP/1.1
Host: api.getfestivo.com
```

## __Response__
* Success
```
{
    "status":200,
    "query":{
        "country":"US",
        "year":"2020"
    },
    "requestId":"681b6098-e38a-4df1-84b3-53fb8d55c523",
    "holidays":[
        {
            "id":"20200101_cd5f5a6c6e09cb5af81af9e87c11a34d",
            "name":"New Year's Day",
            "date":"2020-01-01",
            "observed":"2020-01-01",
            "substitute":false,
            "start":"2020-01-01T00:00:00Z",
            "end":"2020-01-01T23:59:59Z",
            "type":"public"
            ...
        }
    ]
}
```
* Error
```
{
    "error":true,
    "message":"'api_key' is invalid!"
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