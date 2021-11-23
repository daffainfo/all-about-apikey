# [Bitquery](https://graphql.bitquery.io/ide)

## __Description__
Onchain GraphQL APIs & DEX APIs

## __Example Request__
* Curl
```
curl -X POST -H "X-API-KEY: YOURAPIKEY" https://graphql.bitquery.io/
```

* Raw
```
POST / HTTP/1.1
Host: graphql.bitquery.io
X-API-KEY: BQYvhnv04csZHaprIBZNwtpRiDIwEIW9
```

## __Response__
* Success
```
{
    "errors": [{
        "message": "No query string was present"
    }]
}
```
* Error
```
{
    "error": {
        "message": "Invalid or deactivated API key c"
    },
    "data": {}
}
```

## __Regex__
```
[A-Za-z0-9]{32}
```

## __Example API key__
```
LYipNGvE4sHosBhU4tEcTEDrStp3WM5G
```