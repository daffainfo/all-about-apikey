# [Block](https://www.block.io/docs/basic)

## __Description__
Bitcoin Payment, Wallet & Transaction Data

## __Example Request__
* Curl
```
curl 'https://block.io/api/v2/get_balance/?api_key={{token}}'
```

* Raw
```
GET /api/v2/get_balance/?api_key={{token}} HTTP/1.1
Host: block.io
```

## __Response__
* Success
```
{
    "status": "success",
    "data": {
        "network": "BTC",
        "available_balance": "0.00000000",
        "pending_received_balance": "0.00000000"
    }
}
```
* Error
```
{
    "status": "fail",
    "data": {
        "error_message": "API Key invalid or you have not enabled API access for this machine's IP address(es). Check that your API Keys are correct, and that you have enabled API access for this machine's IP Address(es) on your account's Settings page.",
        "connecting_ip": "127.0.0.1"
    }
}
```
## __Regex__
```
[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}
```

## __Example API key__
```
17b5-7e2c-10f1-9eea
```
