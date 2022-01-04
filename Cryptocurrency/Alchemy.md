# [Alchemy](https://docs.alchemy.com/alchemy/)

## __Description__
Ethereum Node-as-a-Service Provider

## __Example Request__
* Curl
```
curl -XPOST "https://eth-mainnet.alchemyapi.io/v2/{{token}}" -d '{"jsonrpc":"2.0","method":"eth_blockNumber","params":[],"id":0}'
```

* Raw
```
POST /v2/{{token}} HTTP/1.1
Host: eth-mainnet.alchemyapi.io
Content-Type: application/x-www-form-urlencoded
Content-Length: 63

{"jsonrpc":"2.0","method":"eth_blockNumber","params":[],"id":0}
```

## __Response__
* Success
```
{
    "jsonrpc": "2.0",
    "id": 0,
    "result": "0x000000"
}
```
* Error
```
{
    "jsonrpc": "2.0",
    "id": 0,
    "error": {
        "code": -32000,
        "message": "Must be authenticated!"
    }
}
```
## __Regex__
```
[a-zA-Z0-9-]{32}
```

## __Example API key__
```
ACf3vvsAUFQ6V4q2ODDDiCf3vvsAsA-a
```
