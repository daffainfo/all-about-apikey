# [Fixer](https://fixer.io/documentation)

## __Description__
Exchange rates and currency conversion

## __Example Request__
* Curl
```
curl "https://data.fixer.io/api/symbols?access_key={{token}}"
```

* Raw
```
GET /api/latest?access_key={{token}} HTTP/1.1
Host: data.fixer.io
...
```

## __Response__
* Success
```
{
    "success": true,
    "symbols": {
        "AED": "United Arab Emirates Dirham",
        "AFN": "Afghan Afghani",
        "ALL": "Albanian Lek",
        "AMD": "Armenian Dram",
        [...]
    }
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
