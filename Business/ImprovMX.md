# [ImprovMX](https://improvmx.com/api)

## __Description__
API for free email forwarding service

## __Example Request__
* Curl
```
curl "https://api.improvmx.com/v3/account" -u ":{{token}}" -L
```

* Raw
```
GET /v3/account HTTP/1.1
Authorization: Basic IDp7e3Rva2VufX0=
Host: api.improvmx.com
```

## __Response__
* Success
```
{
    "account":{
        "billing_email":null,
        "cancels_on":null,
        "card_brand":null,
        "company_details":null,
        "company_name":"test",
        "company_vat":null,
        "country":null,
        "created":1111111111,
        "email":"xxxxxxxxx@gmail.com",
        ...
    }
}
```
* Error
```
{
    "code":401,
    "error":"401 Unauthorized: The server could not verify that you are authorized to access the URL requested. You either supplied the wrong credentials (e.g. a bad password), or your browser doesn't understand how to supply the credentials required.",
    "success":false
}
```

## __Regex__
```
sk_[a-z0-9]{32}
```

## __Example API key__
```
sk_bb1aa18d0eeea0fc7ggg799h3i9578j
```