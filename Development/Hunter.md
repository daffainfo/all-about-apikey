# [Hunter](https://hunter.io/api-documentation/v2)

## __Description__
API for domain search, professional email finder, author finder and email verifier

## __Example Request__
* Curl
```
curl "https://api.hunter.io/v2/domain-search?domain=stripe.com&api_key={{token}}"
```

* Raw
```
GET /v2/domain-search?domain=stripe.com&api_key={{token}} HTTP/1.1
Host: api.hunter.io
```

## __Response__
* Success
```
{
    "data": {
        "domain": "stripe.com",
        "disposable": false,
        "webmail": false,
        "accept_all": true,
        "pattern": "{first}",
        "organization": "Stripe",
        "country": "CA",
        "state": "CA",
        "emails": [
        {
            "value": "christian.anderson@stripe.com",
            "type": "personal",
            "confidence": 99,
            ...
```
* Error
```
{
    "errors": [
        {
        "id": "authentication_failed",
        "code": 401,
        "details": "No user found for the API key supplied"
        }
    ]
}
```
## __Regex__
```
[a-z0-9]{40}
```

## __Example API key__
```
d33bd988d934c09a181c0055f1f387a2ea5978f3
```
