# [Abstract VAT Validation Rates](https://www.abstractapi.com/api/vat-validation-rates-api)

## __Description__
Stay compliant with our simple, reliable, and powerful API for all your domestic and cross-border sales.

## __Example Request__
* Curl
```
curl "https://vat.abstractapi.com/v1/?api_key={{token}}&vat_number=SE556656688001"
```

* Raw
```
GET /v1/?api_key={{token}}&vat_number=SE556656688001 HTTP/1.1
Host: vat.abstractapi.com
```

## __Response__
* Success
```
{
    "vat_number": "SE556656688001",
    "is_vat_valid": true,
    "company_name": "Google Sweden AB",
    "company_address": "Google Ireland Ltd, M Collins, Gordon House, Barrow Street, Dublin 4, Ireland",
    "company_country": "SE",
    "company_country_code": "Sweden"‍
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