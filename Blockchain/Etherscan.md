# [Etherscan](https://docs.etherscan.io/)

## __Description__
Ethereum explorer API

## __Example Request__
* Curl
```
curl -X GET "https://api.etherscan.io/api?module=account&action=balance&address=0xde0b295669a9fd93d5f28d9ec85e40f4cb697bae&tag=latest&apikey=YOURAPIKEY"
```

* Raw
```
GET /api?module=account&action=balance&address=0xde0b295669a9fd93d5f28d9ec85e40f4cb697bae&tag=latest&apikey=YOURAPIKEY HTTP/1.1
Host: api.etherscan.io
```

## __Response__
* Success
```
{
    "status":"1",
    "message":"OK",
    "result":"374868436783144397866641"
}
```
* Error
```
{
    "status":"1",
    "message":"OK-Missing/Invalid API Key, rate limit of 1/5sec applied",
    "result":"374868436783144397866641"
}
```

## __Regex__
```
[A-Z0-9]{34}
```

## __Example API key__
```
47ZBD9SAWKNN6XYB6A92V4GMCC741VYV37
```