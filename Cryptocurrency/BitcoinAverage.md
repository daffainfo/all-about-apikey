# [BitcoinAverage](https://apiv2.bitcoinaverage.com/)

## __Description__
Digital Asset Price Data for the blockchain industry

## __Example Request__
* Curl
```
curl 'https://apiv2.bitcoinaverage.com/exchanges/ticker/bitstamp' -H 'x-ba-key: {{token}}'
```

* Raw
```
GET https://apiv2.bitcoinaverage.com/exchanges/ticker/bitstamp HTTP/1.1
Host: apiv2.bitcoinaverage.com
x-ba-key: {{token}}
```

## __Response__
* Success
```
{
    "name": "bitstamp",
    "display_name": "Bitstamp",
    "url": "https://bitstamp.net/",
    "timestamp": 00000000,
    "data_source": "api",
    "symbols": {
        "ETHUSD": {
            "ask": 0000.00000000,
            "bid": 0000.00000000,
            "last": 0000.000000,
            "high": 0000.000000,
            "low": 000.0000000,
            "open": 0000.000000,
            "vwap": 0000.000000,
            "volume": 000.000000,
            "exchange_symbol": "ETHUSD"
        },
```
* Error
```
Api key does not exist {'xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'}
```
or if expired
```
Your plan has expired. Go to https://pro.bitcoinaverage.com/pages/auth/my-plan to active or extend your plan.
```
## __Regex__
```
[a-zA-Z0-9]{43}
```

## __Example API key__
```
NzI0MjM4Njc1NGQ3NDU4Mzg1NWU3YYmU4MTdiMaADwS
```
