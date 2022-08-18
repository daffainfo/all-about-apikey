# [languagelayer](https://languagelayer.com/documentation)

## __Description__
Language Detection JSON API supporting 173 languages

## __Example Request__
* Curl
```
curl "https://api.languagelayer.com/detect?access_key={{token}}&query=The%20pessimist%20complains%20about%20the%20wind%3B%20the%20optimist%20expects%20it%20to%20change%3B%20the%20realist%20adjusts%20the%20sails"
```

* Raw
```
GET /detect?access_key={{token}}&query=The%20pessimist%20complains%20about%20the%20wind%3B%20the%20optimist%20expects%20it%20to%20change%3B%20the%20realist%20adjusts%20the%20sails HTTP/1.1
Host: api.languagelayer.com
...
```

## __Response__
* Success
```
{
    "success": true,
    "results": [
        {
        "language_code": "en",
        "language_name": "English",
        "probability": 83.896703655741,
        "percentage": 100,
        "reliable_result": true
        }
    ]
}
```
* Error
```
{
    "success": false,
    "error": {
        "code": 101,
        "type": "invalid_access_key",
        "info": "You have not supplied a valid API Access Key. [Technical Support: support@apilayer.com]"
    }
}
```
## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
tue3sv9hzsey1me4l7fwq3t46u5k8wag
```
