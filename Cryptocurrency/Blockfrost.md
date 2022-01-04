# [Blockfrost](https://docs.blockfrost.io/)

## __Description__
Interaction with the Cardano mainnet and several testnets

## __Example Request__
* Curl
```
curl -H "project_id: {{token}}" "https://cardano-mainnet.blockfrost.io/api/v0/"
```

* Raw
```
GET /api/v0/ HTTP/1.1
Host: cardano-mainnet.blockfrost.io
project_id: {{token}}
```

## __Response__
* Success
```
{
    "url":"https://blockfrost.io/",
    "version":"0.16.4"
}
```
* Error
```
{
    "status_code":403,
    "error":"Forbidden",
    "message":"Invalid project token."
}
```
## __Regex__
* Mainnet
```
mainnet[a-zA-Z0-9]{32}
```
* Testnet
```
testnet[a-zA-Z0-9]{32}
```
* IPFS
```
ipfs[a-zA-Z0-9]{32}
```

## __Example API key__
```
* Mainnet
```
mainnet8tc4fJ1ddM2VmnbFzTk3f7hXsrehnT8w
```
* Testnet
```
testnet8tc4fJ1ddM2VmnbFzTk3f7hXsrehnT8w
```
* IPFS
```
ipfs8tc4fJ1ddM2VmnbFzTk3f7hXsrehnT8w
```