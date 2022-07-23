# [Bitrise](https://api-docs.bitrise.io/)

## __Description__
Build tool and processes integrations to create efficient development pipelines

## __Example Request__
* Curl
```
curl "https://api.bitrise.io/v0.1/me" -H "Authorization: {{token}}"
```

* Raw
```
GET /v0.1/me HTTP/1.1
Host: api.bitrise.io
Authorization: {{token}}
```

## __Response__
* Success
```
{
    "data":{
        "username":"test",
        "slug":"xxxxxxxxxxxx",
        "email":"test@gmail.com",
        "avatar_url":"",
        "created_at":"2021-12-17T13:56:19.925193Z",
        "has_used_organization_trial":false,
        "data_id":12345,
        "payment_processor":"Stripe"
    }
}
```
* Error
```
{
    "message":"Unauthorized"
}
```
## __Regex__
```
[a-zA-Z0-9-_]{86}
```

## __Example API key__
```
Xx123X330-XxXxX1234567_XxXxX1234567XxXxX1234567XxXxX1234567XxXxX12_XxXxX1234567XxXxX1
```
