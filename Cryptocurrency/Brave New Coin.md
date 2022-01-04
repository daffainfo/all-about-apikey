# [Brave New Coin](https://bravenewcoin.com/developers)

## __Description__
Real-time and historic crypto data from more than 200+ exchanges

## __Example Request__
* Curl
```
curl --request GET \
	--url https://bravenewcoin.p.rapidapi.com/market \
	--header 'x-rapidapi-host: bravenewcoin.p.rapidapi.com' \
	--header 'x-rapidapi-key: {{token}}'
```

* Raw
```
GET /market HTTP/1.1
X-Rapidapi-Host: bravenewcoin.p.rapidapi.com
X-Rapidapi-Key: {{token}}
Host: bravenewcoin.p.rapidapi.com
```

## __Response__
* Success
```
{
    "content": [{
        "id": "xxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
        "baseAssetId": "xxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
        "quoteAssetId": "xxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
    }, {
        "id": "xxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
        "baseAssetId": "xxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx",
        "quoteAssetId": "xxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx"
    },
    ...
}
```
* Error
```
{
    "message":"You are not subscribed to this API."
}
```
## __Regex__
```
[a-z0-9]{50}
```

## __Example API key__
```
d2vr0v1r039rik1293r9v3rk1i2ix239ri2309ri20r9i32r2r
```