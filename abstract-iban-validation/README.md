# [Abstract IBAN Validation](https://www.abstractapi.com/api/iban-validation)

## __Description__
A powerful REST API to validate IBAN quickly and securely

## __Example Request__
* Curl
```
curl "https://ibanvalidation.abstractapi.com/v1/?api_key={{token}}&iban=BE71096123456769"
```

* Raw
```
GET /v1/?api_key={{token}}&iban=BE71096123456769 HTTP/1.1
Host: ibanvalidation.abstractapi.com
```

## __Response__
* Success
```
{
    "iban": "BE71096123456769",
    "is_valid": true
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