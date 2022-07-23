# [Clockify](https://clockify.me/developers-api)

## __Description__
Clockify's REST-based API can be used to push/pull data to/from it & integrate it with other systems

## __Example Request__
* Curl
```
curl -H "Content-Type: application/json" -H "X-Api-Key: {{token}}" -X GET https://api.clockify.me/api/v1/user
```

* Raw
```
GET /api/v1/user HTTP/1.1
Host: api.clockify.me
X-Api-Key: {{token}}
Content-Type: application/json
```

## __Response__
* Success
```
{
    "id":"qwertyuiop98fc8f836af59327f",
    "email":"luisjivillalba@gmail.com",
    "name":"Luis Juan Ignacio Villalva",
    "memberships":[],
    "profilePicture":"https://img.clockify.me/no-user-image.png",
    "activeWorkspace":"qwertyuiopa8fc8f836af593x",
    "defaultWorkspace":"qwertyuiopa8fc8f836af593x",
    "settings":{
        "weekStart":"MONDAY",
        "timeZone":"America/Buenos_Aires",
        "timeFormat":"HOUR24",
        "dateFormat":"DD/MM/YYYY",
        "sendNewsletter":false,
        "weeklyUpdates":false,
        "longRunning":false,
        "scheduledReports":true,
        ...
    }
}
```
* Error
```
{
    "message":"Api key does not exist",
    "code":4003
}
```
## __Regex__
```
[a-zA-Z0-9]{48}
```

## __Example API key__
```
YQ6wba4vACaht9CUK9k5N7QxV2ieRPJ396g94vkWSYauYmch
```
