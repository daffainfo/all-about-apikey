# [AbuseIPDB](https://docs.abuseipdb.com/)

## __Description__
IP/domain/URL reputation

## __Example Request__
* Curl
```
curl https://api.abuseipdb.com/api/v2/report \
  --data-urlencode "ip=127.0.0.1" \
  -d categories=18,22 \
  --data-urlencode "comment=SSH login attempts with user root." \
  -H "Key: $YOUR_API_KEY" \
  -H "Accept: application/json"
```

* Raw
```
POST /api/v2/report HTTP/1.1
Host: api.abuseipdb.com
Key: $YOUR_API_KEY
Accept: application/json
Content-Type: application/x-www-form-urlencoded
Content-Length: 16

ip=127.0.0.1&categories=18,22&comment=SSH%20login%20attempts%20with%20user%20root.
```

## __Response__
* Success
```
  {
    "data": {
      "ipAddress": "127.0.0.1",
      "abuseConfidenceScore": 52
    }
  }
```
* Error
```
{
    "errors": [{
        "detail": "Authentication failed. Your API key is either missing, incorrect, or revoked. Note: The APIv2 key differs from the APIv1 key.",
        "status": 401
    }]
}
```

## __Regex__
```
[a-z0-9]{80}
```

## __Example API key__
```
c3k69z846qn30q4r6eo3gsg3urqanuoypyluil350m7iyyw55mx6hd22aaa7xj9y0xbk2ygtrcxuzbh8
```