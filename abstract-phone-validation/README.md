# [Abstract Phone Validation](https://www.abstractapi.com/api/phone-validation-api)

## __Description__
Improve your contact rate and clean your lists with Abstract's industry-leading phone number validation API

## __Example Request__
* Curl
```
curl "https://phonevalidation.abstractapi.com/v1/?api_key={{token}}&number=14154582468"
```

* Raw
```
GET /v1/?api_key={{token}}&number=14154582468 HTTP/1.1
Host: phonevalidation.abstractapi.com
```

## __Response__
* Success
```
{
    "number": "14154582468",
    "is_valid_number": true,
    "local_format":"4154582468",
    "international_format": "+14154582468",
    "country_name": "United States of America",
    "country_code": "US",
    "country_prefix":"+1",
    "registered_location": "San Francisco, CA",
    "carrier":"Verizon USA",
    "line_type": "Mobile",
}
```
* Error
```
{
    "error":{
        "message":"Invalid API key provided.",
        "code":"unauthorized",
        "details":null
    }
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