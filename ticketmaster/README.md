# [Ticketmaster](http://developer.ticketmaster.com/products-and-docs/apis/getting-started/)

## __Description__
Search events, attractions, or venues

## __Example Request__
* Curl
```
curl "https://app.ticketmaster.com/discovery/v2/events.json?apikey={{token}}"
```

* Raw
```
GET /discovery/v2/events.json?apikey={{token}} HTTP/1.1
Host: app.ticketmaster.com
```

## __Response__
* Success
```
{
    "_embedded":{
        "events":[
            {
                "name":"Imagine Dragons: Mercury World Tour",
                "type":"event",
                "id":"Z7r9jZ1Ad8S4v",
                "test":false,
                "url":"https://www.ticketmaster.com/event/abcd1234avcd",
                "locale":"en-us",
                "images":[
                    {
                        "ratio":"16_9",
                        ...
                    }
                ]
            }
        ]
    }
}
```
* Error
```
{
    "fault": {
        "faultstring": "Invalid ApiKey",
        "detail": {
            "errorcode": "oauth.v2.InvalidApiKey"
        }
    }
}
```
## __Regex__
```
[a-zA-Z0-9]{32}
```

## __Example API key__
```
QSzFlcDwaXtfevSu4Oo98AsJb4fKMGio
```