# [Blitapp](https://blitapp.com/api/)

## __Description__
Schedule screenshots of web pages and sync them to your cloud

## __Example Request__
* Curl
```
curl -X GET "https://blitapp.com/api/scheduledcapture" -H "accept: application/json" -H "Api-key: {{token}}"
```

* Raw
```
GET /api/scheduledcapture HTTP/1.1
Host: blitapp.com
Accept: application/json
Api-key: {{token}}
```

## __Response__
* Success
```
[
    {
        "id": "204347e0-eaf8-11e9-ac83-338a9cee6792",
        "name": "My capture",
        "paused": true,
        "comment": "string",
        "createdAt": "2019-10-09T02:43:15.281Z",
        "updatedAt": "2019-10-09T02:43:15.281Z",
        "captureRequest": {
        "apps": [
            "204347e0-eaf8-11e9-ac83-338a9cee6792"
        ],
        "browser": "Chrome",
        "country": "USA",
        "cropHeight": null,
        "cropLeft": 0,
        "cropTop": 0,
        "cropBottom": null,
        "emails": [
            "foo@gmail.com"
        ],
```
* Error
```
{
    "errorType":"NotAuthorized",
    "properties":{},
    "requestId":"abcd1234-1234-asdf-1234-asdfqwer1234"
}
```
## __Regex__
```
[a-zA-Z0-9-_.~]{35,48}
```

## __Example API key__
```
jWksobI15SXxc7_s8vPtr.NX0bD2OvFFcBWG6P
Xc7h5o9zEg5WW1W1uZBbvbHF1m_ac-AHLhBEyo
3WJU7RRjWdZbyzvelY4_VwA4vcYCEe4QT4e7pl6
v1ZhaaZLrI8wdPnwpf1ucKryQHVCqVPpa.hrLTTSQVydwwA-
fxy3qmsBVH~uH89qrXVv8qYQ_LA.sfknXEP2~.COxz
Y_m6gs3GjpemJratcwED~c8wanEIH-nrupZr~sT
B-plC0dnF5_jjIUe_FNXlSTqMi6mEjZZB9jYRdsYcAzM
```
