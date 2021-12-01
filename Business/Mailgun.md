# [Mailgun](https://www.mailgun.com/)

## __Description__
Email Service

## __Example Request__
* Curl
```
curl -s --user 'api:{{token}}' -G \
    https://api.mailgun.net/v3/domains \
    -d skip=0 \
    -d limit=3
```

* Raw
```
POST /v3/domains HTTP/1.1
Authorization: Basic YXBpOnt7dG9rZW59fQ==
Host: api.mailgun.net
Content-Type: application/x-www-form-urlencoded
Content-Length: 14

skip=0&limit=3
```

## __Response__
* Success
```
{
  "items": [
    {
      "created_at": "Thu, 01 May 2021 10:10:10 GMT",
      "id": "xxxxxxxx",
      "is_disabled": false,
      "name": "test.com",
      "require_tls": false,
      "skip_verification": false,
      "smtp_login": "test@test.com",
      "spam_action": "disabled",
      "state": "unverified",
      "type": "custom",
      "web_prefix": "email",
      "web_scheme": "http",
      "wildcard": false
    },
    ...
  ],
  "total_count": 2
}
```
* Error
```
{
    "message":"Invalid private key"
}
```

## __Regex__
```
key-[a-z0-9]{32}
```

## __Example API key__
```
key-bb1aa18d0eeea0fc7ggg799h3i9578j
```