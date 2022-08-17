# [Aletheia](https://aletheiaapi.com/docs/)

## __Description__
Insider trading data, earnings call analysis, financial statements, and more

## __Example Request__
* Curl
```
curl "http://api.aletheiaapi.com/LatestTransactions?issuer=TSLA&owner=1494730" -H "Key: {{token}}"
```

* Raw
```
GET /LatestTransactions?issuer=TSLA&owner=1494730 HTTP/1.1
Host: api.aletheiaapi.com
Key: {{token}}
```

## __Response__
* Success
```
[
    {
        "Id":"abcd1234-abcd-1234-abcd-abcd1234abcd",
        "FromFiling":"abcd1234-abcd-1234-abcd-abcd1234abcd",
        "EntryType":0,
        "QuantityOwnedFollowingTransaction":166587740.0,
        "Direcn Stock",
        "SecurityType":0,
        "AcquiredDisposed":1,
        "Quantity":28526.0,
        "PricePerSecurity":null,
        "TransactionDate":"2022-04-28T00:00:00",
        ...
    }
]
```
* Error
```
API key invalid
```
## __Regex__
```
[A-Z0-9]{32}
```

## __Example API key__
```
LGIWODLS8P9IHLTAC5WL1JDKWIE1ABCD
```