# [MailboxValidator](https://www.mailboxvalidator.com/api-email-free)

## __Description__
Validate email address to improve deliverability

## __Example Request__
* Curl
```
curl https://api.mailboxvalidator.com/v1/email/free?email=test@test.com&key={{token}}
```

* Raw
```
GET /v1/email/free?email=test@test.com&key={{token}} HTTP/1.1
Host: api.mailboxvalidator.com
```

## __Response__
* Success
```
{
    "email_address":"test@test.com",
    "is_free":"False",
    "credits_available":999,
    "error_code":"",
    "error_message":""
}
```
* Error
```
{
    "email_address":"",
    "is_free":"",
    "credits_available":"",
    "error_code":"101",
    "error_message":"API key not found."
}
```

## __Regex__
```
[A-Z0-9]{20}
```

## __Example API key__
```
1MA2C3BBBASAAAA6AA77
```