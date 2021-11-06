# [Covalent](https://www.covalenthq.com/docs/api/)

## __Description__
Multi-blockchain data aggregator platform

## __Example Request__
* Curl
```
curl -X GET "https://api.covalenthq.com/v1/3/address/balances_v2/?&key=YOURAPIKEY" -H "Accept: application/json"
```

* Raw
```
GET /v1/3/address/balances_v2/?&key=YOURAPIKEY HTTP/1.1
Host: api.covalenthq.com
Accept: application/json
```

## __Response__
* Success
```
{
  "address": "string",
  "updated_at": "1970-01-01T00:00:00.000Z",
  "next_update_at": "1970-01-01T00:00:00.000Z",
  "quote_currency": "string",
  "uniswap_v2": {
    "balances": [
      {
        "token_0": {
          "contract_decimals": 0,
          "contract_ticker_symbol": "string",
          "contract_address": "string",
          "logo_url": "string",
          "balance": 0,
          "quote": 0.5,
          "quote_rate": 0.5
        }
        ...
      }
    ]
  }
}
```
* Error
```
{
    "data":null,
    "error":true,
    "error_message":"Invalid API key",
    "error_code":401
}
```

## __Regex__
```
ckey_[a-z0-9]{27}
```

## __Example API key__
```
ckey_9c452a7xxxxxxb94832cxxxffff
```