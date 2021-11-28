# [Clearbit](https://clearbit.com/docs)

## __Description__
Search for company logos and embed them in your projects

## __Example Request__
* Curl
```
curl "https://person.clearbit.com/v2/combined/find?email=alex@clearbit.com" -u {{token}}:
```

* Raw
```
GET /v2/combined/find?email=alex@clearbit.com HTTP/1.1
Authorization: Basic e3t0b2tlbn19Og==
Host: person.clearbit.com
```

## __Response__
* Success
```
{
  "person": {
    "id": "3622a31e-7d4c-41bf-a422-65b36b4a401d",
    "name": {
      "fullName": "Alex MacCaw",
      "givenName": "Alex",
      "familyName": "MacCaw"
    },
    "email": "alex@clearbit.com",
    "location": "San Francisco, CA, US",
    "timeZone": "America/Los_Angeles",
    "utcOffset": -8,
```
* Error
```
{
    "error":{
        "type":"invalid_api_key",
        "message":"Invalid API key provided"
    }
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