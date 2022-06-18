# [Api2Convert](https://www.api2convert.com/docs/index.html)

## __Description__
Online File Conversion API

## __Example Request__
* Curl
```
curl -X POST \
    https://api.api2convert.com/v2/jobs \
    -H 'cache-control: no-cache' \
    -H 'content-type: application/json' \
    -H 'x-oc-api-key: {{token}}' \
    -d '{
           "input": [{
               "type": "remote",
               "source": "https://example-files.online-convert.com/raster%20image/png/example_small.png"
           }],
           "conversion": [{
               "category": "image",
               "target": "png"
           }],
           "callback": "https://my.domain.test/apiCallback"
       }'
```

* Raw
```
POST /v2/jobs HTTP/1.1
Host: https://api.api2convert.com
X-Oc-Api-Key: {{token}}
Content-Type: application/json
{
    "input": [{
        "type": "remote",
        "source": "https://example-files.online-convert.com/raster%20image/jpg/example_small.jpg"
    }],
    "conversion": [{
        "target": "png"
    }]
}
```

## __Response__
* Success
```
{
    "id": "xxxxxxx-027b-483e-bac9-9311fe4764b9",
    "token": "xxxxxxxee5a986b35b96c78f60eab8c2",
    "type": "job",
    "status": {
        "code": "downloading",
        "info": "The file is currently downloading from the source URL."
    },
    "errors": [],
    "process": true,
    "conversion": [
        {
            ... information about conversion ...
        }
    ],
    "input": [
        {
            ... information about the input ...
        }
    ],
    "output": [],
    "callback": "",
    "notify_status": false,
    "server": "https://www27.api2convert.com/v2/dl/web2",
    "spent": 0,
    "created_at": "2017-08-15T17:20:55",
    "modified_at": "2017-08-15T17:20:55"
}
```
* Error
```
{
    "message":"Invalid api key"
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
