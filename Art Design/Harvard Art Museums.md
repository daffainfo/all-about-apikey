# [Harvard Art Museums](https://github.com/harvardartmuseums/api-docs)

## __Description__
Harvard Art

## __Example Request__
* Curl
```
https://api.harvardartmuseums.org/color/34838442?apikey=YOURAPIKEY
```

* Raw
```
GET /color/34838442?apikey=YOURAPIKEY HTTP/1.1
Host: api.harvardartmuseums.org
```

## __Response__
* Success
```
{
    "colorid":34838442,
    "name":"darksalmon",
    "hex":"#e9967a",
    "id":34838442,
    "lastupdate":"2021-11-10T04:16:54-0500"
}
```
* Error
```
Unauthorized
```

## __Regex__
```
[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}
```

## __Example API key__
```
c8267d84-db73-5b90-b8c4-e17b456857b8
```