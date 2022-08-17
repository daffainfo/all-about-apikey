# [SeatGeek](https://platform.seatgeek.com/)

## __Description__
Search events, venues and performers

## __Example Request__
* Curl
```
curl "https://api.seatgeek.com/2/events?client_id={{token}}"
```

* Raw
```
GET /2/events?client_id={{token}} HTTP/1.1
Host: api.seatgeek.com
```

## __Response__
* Success
```
{
    "events":[
        {
            "type":"minor_league_baseball",
            "id":5576169,
            "datetime_utc":"2022-08-17T08:30:00",
            "venue":{
                "state":"KY",
                "name_v2":"Bowling Green Ballpark",
                "postal_code":"42101",
                "name":"Bowling Green Ballpark",
                "links":[],
                "timezone":"America\/Chicago",
                ...
            }
        }
    ]
}
```
* Error
```
{
    "status":403,
    "message":"Invalid client credentials",
    "errors":[
        {
            "message":"Invalid client credentials",
            "code":40302
        }
    ],
    "meta":{
        "status":403
    }
}
```
## __Regex__
```
MjM[a-zA-Z0-9]{33}
```

## __Example API key__
```
MjM4MDc2NjV8MTU3MDQ4otQ1MC45MQfk12MK
```