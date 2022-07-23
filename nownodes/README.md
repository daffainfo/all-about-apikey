# [Nownodes](https://nownodes.io/)

## __Description__
Blockchain-as-a-service solution that provides high-quality connection via API

## __Example Request__
* Curl
```
curl --location --request GET 'https://bsc-blockbook.nownodes.io/api' \
--header 'api-key: YOURAPIKEY' \
--header 'Content-Type: application/json'
```

* Raw
```
GET /api HTTP/1.1
Host: bsc-blockbook.nownodes.io
api-key: YOURAPIKEY
Content-Type: application/json
```

## __Response__
* Success
```
{
    "blockbook":{
        "coin":"BSC",
        "host":"full-nodes-75d416b6",
        "version":"devel",
        "gitCommit":"4534817-dirty",
        ...
        "decimals":18,
        "dbSize":231263470422,
        "about":"Blockbook - blockchain indexer for Trezor wallet https://trezor.io/. Do not use for any other purpose."
        },
        "backend":{
            "chain":"mainnet",
            "blocks":12405155,"bestBlockHash":"0x95b790cb97405453e66d2f19366644c638cd5826d96570f5e9c387d5e3630b33",
            "difficulty":"2",
            "version":"Geth/v1.1.2-c4f93121/linux-amd64/go1.15.5"
        }
    }
```
* Error
```
{
    "message":"Unknown API_key"
}
```

## __Regex__
```
[A-Za-z0-9]{32}
```

## __Example API key__
```
MrID9UAAildWnSbukhzdQA2YA1u9shld
```