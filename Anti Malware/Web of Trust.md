# [Web of Trust](https://support.mywot.com/hc/en-us/sections/360004477734-API-)

## __Description__
IP/domain/URL reputation

## __Example Request__
* Curl
```
curl -H "x-user-id: USERID" -H "x-api-key: YOURAPIKEY" -X GET "https://scorecard.api.mywot.com/v3/targets?t=hbo.com&t=google.com"
```

* Raw
```
GET /v3/targets?t=hbo.com&t=google.com HTTP/1.1
Host: scorecard.api.mywot.com
x-user-id: USERID
x-api-key: YOURAPIKEY
```

## __Response__
* Success
```
[
    {
        "target":"hbo.com",
        "safety":{
            "status":"SAFE",
            "reputations":93,
            "confidence":59
        },"childSafety":{
            "reputations":90,
            "confidence":52
        },"categories":[
            {
                "id":501,
                "name":"good site",
                ...
            }
        ]
    }
]
```
* Error
```
```
> No output if error

## __Regex__
* User ID
```
[0-9]{7}
```
* API Key
```
[a-z0-9]{40}
```

## __Example key__
* User ID
```
1234567
```
* API Key
```
tue3sv9hzsey1me4l7fwq3t46u5k8wagabcdefgh
```