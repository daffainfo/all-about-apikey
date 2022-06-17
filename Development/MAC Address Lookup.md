# [MAC Address Lookup](https://macaddress.io/api)

## __Description__
Retrieve vendor details and other information regarding a given MAC address or an OUI

## __Example Request__
* Curl
```
curl "https://api.macaddress.io/v1?apiKey={{token}}&output=json&search=44:38:39:ff:ef:57"
```

* Raw
```
GET /v1?apiKey={{token}}&output=json&search=44:38:39:ff:ef:57 HTTP/1.1
Host: api.macaddress.io
```

## __Response__
* Success
```
{
    "vendorDetails":{
        "oui":"443839",
        "isPrivate":false,
        "companyName":"Cumulus Networks, Inc",
        "companyAddress":"650 Castro Street, suite 120-245 Mountain View CA 94041 US",
        "countryCode":"US"},
        "blockDetails":{
            "blockFound":true,
            "borderLeft":"443839000000",
            "borderRight":"443839FFFFFF",
            "blockSize":16777216,
            ...
```
* Error
```
{
    "error":"Access restricted. Enter the correct API key."
}
```
## __Regex__
```
at_[a-zA-Z0-9]{29}
```

## __Example API key__
```
at_Fa2SfmKp3gkLD1PqoLfowkOts7pl3y
```
