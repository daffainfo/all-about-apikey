# [Abstract Email Validation](https://www.abstractapi.com/api/email-verification-validation-api)

## __Description__
Improve your delivery rate and clean your email lists with Abstract's industry-leading email verification API

## __Example Request__
* Curl
```
curl "https://emailvalidation.abstractapi.com/v1/?api_key={{token}}&email=johnsmith@gmail.com"
```

* Raw
```
GET /v1/?api_key={{token}}&email=johnsmith@gmail.com HTTP/1.1
Host: emailvalidation.abstractapi.com
```

## __Response__
* Success
```
{
    "email": "johnsmith@gmail.com",
    "autocorrect": "",
    "is_valid_format": true,
    "is_free_email": true,
    "is_disposable_email": false,
    "is_role_email": false,
    "is_catchall_email": false,
    "is_mx_found": true,
    "is_smtp_valid": true,
    "quality_score": 0.99,
}
```
* Error
```
{
    "error":{
        "message":"Invalid API key provided.",
        "code":"unauthorized",
        "details":null
    }
}
```

## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
of3ab02f3xd12ldofxc3fosc129sd241
```