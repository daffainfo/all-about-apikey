# [IP2WHOIS](https://www.ip2whois.com/developers-api)

## __Description__
WHOIS domain name lookup

## __Example Request__
* Curl
```
curl "https://api.ip2whois.com/v2?key={{token}}&domain=daffa.tech&format=json"
```

* Raw
```
GET /v2?key={{token}}&domain=daffa.tech&format=json HTTP/1.1
Host: api.ip2whois.com
```

## __Response__
* Success
```
{
    "domain":"daffa.tech",
    "domain_id":"D205554988-CNIC",
    "status":"clientTransferProhibited https://icann.org/epp#clientTransferProhibited",
    "create_date":"2020-10-23T06:03:38+00:00",
    "update_date":"2021-09-06T07:38:48+00:00",
    "expire_date":"2022-10-23T23:59:59+00:00",
    "domain_age":602,
    "whois_server":"whois.hostinger.com"
    ...
```
* Error
```
{
    "error":{
        "error_code":10001,
        "error_message":"API key not found."
    }
}
```
## __Regex__
```
[A-Z0-9]{32}
```

## __Example API key__
```
LGIWODLS8P9IHLTAC5WL1JDKWIE1ABCD
```
