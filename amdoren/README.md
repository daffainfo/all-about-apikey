# [Amdoren](https://www.amdoren.com/currency-api/)

## __Description__
Free currency API with over 150 currencies

## __Example Request__
* Curl
```
curl "https://www.amdoren.com/api/currency.php?api_key={{token}}&from=USD&to=EUR"
```

* Raw
```
GET /api/currency.php?api_key={{token}}&from=USD&to=EUR HTTP/1.1
Host: www.amdoren.com
```

## __Response__
* Success
```
{
    "error" : 0,
    "error_message" : "-",
    "amount" : 0.95356
}
```
* Error
```
{
    "error" : 110,
    "error_message" : "Invalid API key: {{token}}.",
    "amount" : 0
}
```
## __Regex__
```
[a-zA-Z0-9]{30}
```

## __Example API key__
```
QSzFlcDwaXtfevSu4Oo98AsJb4fKMG
```
