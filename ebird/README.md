# [eBird](https://documenter.getpostman.com/view/664302/S1ENwy59)

## __Description__
Retrieve recent or notable birding observations within a region

## __Example Request__
* Curl
```
curl --location --request GET "https://api.ebird.org/v2/data/obs/KZ/recent" --header "X-eBirdApiToken: {{APIKEY}}"
```

* Raw
```
GET /v2/data/obs/KZ/recent HTTP/1.1
Host: api.ebird.org
X-eBirdApiToken: {{APIKEY}}
```

## __Response__
* Success
```
[
    {
        "speciesCode":"gretit1",
        "comName":"Great Tit",
        "sciName":"Parus major",
        "locId":"L14009371",
        "locName":"Atyrau Yard",
        "obsDt":"2021-11-11 13:39",
        "howMany":4,"lat":47.101336,
        "lng":51.91241,
        "obsValid":true,
        "obsReviewed":false,
        "locationPrivate":true,
        "subId":"S97421089"
    },
    {
        "speciesCode":"casgul2",
        "comName":"Caspian Gull",
        "sciName":"Larus cachinnans",
        ...
    }
]
```
* Error
```

```
> No output if APIKEY is wrong

## __Regex__
```
[a-z0-9]{12}
```

## __Example API key__
```
19jf092v8gpl
```