# [Europeana](https://pro.europeana.eu/page/search)

## __Description__
European Museum and Galleries content

## __Example Request__
* Curl
```
curl "https://api.europeana.eu/record/v2/search.json?wskey=APIKEY&query=*&rows=0&profile=facets"
```

* Raw
```
GET /record/v2/search.json?wskey=APIKEY&query=*&rows=0&profile=facets HTTP/1.1
Host: api.europeana.eu
```

## __Response__
* Success
```
{
    "apikey":"APIKEY",
    "success":true,
    "requestNumber":999,
    "itemsCount":0,
    "totalResults":62396081,
    "items":[],
    .....
}
```
* Error
```
{
    "apikey":"APIKEY",
    "success":false,
    "error":"API key doesn't exist",
    "code":"401-AX"
}
```

## __Regex__
```
[a-z]{8,10}
```

## __Example API key__
```
fvvxvpdp
haakaofij
bjgqtpybnr
```