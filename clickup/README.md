# [ClickUp](https://clickup.com/api)

## __Description__
ClickUp is a robust, cloud-based project management tool for boosting productivity

## __Example Request__
* Curl
```
curl "https://api.clickup.com/api/v2/user" -H "Authorization: {{token}}"
```

* Raw
```
GET /api/v2/user HTTP/1.1
Host: api.clickup.com
Authorization: {{token}}
...
```

## __Response__
* Success
```
{
    "user":{
        "id": 1234567,
        "username":"test",
        "email":"test@gmail.com",
        "color":"#8ac34a",
        "profilePicture":null,
        "initials":"t",
        "week_start_day":null,
        "global_font_support":true,
        "timezone":"Asia/Bangkok"
    }
}
```
* Error
```
{
    "err":"Token invalid","ECODE":"OAUTH_025"
}
```
## __Regex__
```
pk_[0-9]{8}_[0-9A-Z]{32}
```

## __Example API key__
```
pk_45325102_1FL26CQT2M1VG83CNL2RSE2IMFN64D9A
```
