# [Charity Search](http://charityapi.orghunter.com/)

## __Description__
Non-profit charity data

## __Example Request__
* Curl
```
curl "http://data.orghunter.com/v1/charitybasic?user_key=YOURAPIKEY&ein=590774235"
```

* Raw
```
GET /v1/charitybasic?user_key=YOURAPIKEY&ein=590774235 HTTP/1.1
Host: data.orghunter.com
```

## __Response__
* Success
```
{
    "code":200,
    "msg":"OK, all went through!",
    "data":
    {
        "ein":"590774235",
        "name":"HUMANE SOCIETY OF THE TREASURE COAST INC",
        "inCareOfName":"",
        "street":"4100 SW LEIGHTON FARM AVE",
        "city":"PALM CITY",
        "state":"FL",
        "zipCode":"34990-5623",
        "country":"USA",
        "groupExemption":null,
        ...
    }
}
```
* Error
```
{
    "code":"403",
    "msg":"Unauthorized"
}
```

## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
q7uy1n2sdk26e72fv91yrlb086ybqex6
```