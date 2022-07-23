# [Calendarific](https://calendarific.com/api-documentation)

## __Description__
Worldwide Holidays

## __Example Request__
* Curl
```
curl "https://calendarific.com/api/v2/holidays?api_key={{token}}&country=US&year=2021"
```

* Raw
```
GET /api/v2/holidays?api_key={{token}}&country=US&year=2021 HTTP/1.1
Host: calendarific.com
```

## __Response__
* Success
```
{
    "meta":{
        "code":200
    },
    "response":{
        "holidays":[{
            "name":"New Year's Day",
            "description":"New Year's Day is the first day of the Gregorian calendar, which is widely used in many countries such as the USA.",
            "country":{
                "id":"us",
                "name":"United States"
            },
            "date":{
                "iso":"2021-01-01",
                "datetime":{
                    "year":2021,
                    "month":1,"day":1
                    }
                },
                ...
```
* Error
```
{
    "meta":{
        "code":401,
        "error_type":"auth failed",
        "error_detail":"Missing or invalid api credentials. See https:\/\/calendarific.com\/api for details."
        },
    "response":[]
}
```

## __Regex__
```
[a-z0-9]{40}
```

## __Example API key__
```
fb928595c436941d6cbbcd4b408vk49d3993312d
```
