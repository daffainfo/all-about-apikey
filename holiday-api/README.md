# [Holiday API](https://holidayapi.com/docs)

## __Description__
Historical data regarding holidays

## __Example Request__
* Curl
```
curl "https://holidayapi.com/v1/holidays?pretty&key={{token}}&country=US&year=2020&language=EN"
```

* Raw
```
GET /v1/holidays?pretty&key={{token}}&country=US&year=2020&language=EN HTTP/1.1
Host: holidayapi.com
```

## __Response__
* Success
```
{
    "status": 200,
    "warning": "These results do not include state and province holidays. For more information, please visit https:\/\/holidayapi.com\/docs",
    "requests": {
        "used": 167,
        "available": 9833,
        "resets": "2021-12-01 00:00:00"
    },
    "holidays": [
        {
            "name": "New Year's Day",
            "date": "2020-01-01",
            "observed": "2020-01-01",
            "public": true,
            "country": "US",
            "uuid": "82f78b8a-019e-479e-a19f-99040275f9bf",
            "weekday": {
                "date": {
                    "name": "Wednesday",
                    "numeric": "3"
                },
                "observed": {
                    "name": "Wednesday",
                    "numeric": "3"
                }
            }
        },
        {
            "name": "Seventh Day of Kwanzaa",
            "date": "2020-01-01",
            "observed": "2020-01-01",
            "public": false,
            "country": "US",
            "uuid": "0e766ff3-0d31-40e1-85e1-49ed61ab006d",
            "weekday": {
                "date": {
                    "name": "Wednesday",
                    "numeric": "3"
                },
                "observed": {
                    "name": "Wednesday",
                    "numeric": "3"
                }
            }
        }
        ...
```
* Error
```
{
    "status": 401,
    "error": "Invalid API key. For more information, please visit https:\/\/holidayapi.com\/docs"
}
```

## __Regex__
```
[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}
```

## __Example API key__
```
c8267d84-db73-5b90-b8c4-e17b456857b8
```