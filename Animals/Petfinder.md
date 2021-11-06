# [Petfinder](https://www.petfinder.com/developers/v2/docs/)

## __Description__
Petfinder is dedicated to helping pets find homes, another resource to get pets adopted

## __Example Request__
* Curl
```
curl -d "grant_type=client_credentials&client_id=CLIENT-ID&client_secret=CLIENT-SECRET" https://api.petfinder.com/v2/oauth2/token
```

* Raw
```
POST /v2/oauth2/token HTTP/1.1
Host: api.petfinder.com
Content-Type: application/x-www-form-urlencoded
Content-Length: 81

grant_type=client_credentials&client_id=CLIENT-ID&client_secret=CLIENT-SECRET
```

## __Response__
* Success
```
{
    "token_type":"Bearer",
    "expires_in":3600,
    "access_token":"eyJ0eXxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
}
```
* Error
```
{
  "type": "https://www.petfinder.com/developers/v2/docs/errors/ERR-401/",
  "status": 401,
  "title": "invalid_client",
  "detail": "Client authentication failed",
  "errors": [
    {
      "code": "invalid_client",
      "title": "Unauthorized",
      "message": "Client authentication failed",
      "details": "Client authentication failed",
      "href": "http://developer.petfinder.com/v2/errors.html#invalid_client"
    }
  ],
  "hint": null
}
```

## __Regex__
* Client ID / API Key
```
[a-zA-Z0-9]{50}
```
* Client Secret
```
[a-zA-Z0-9]{40}
```

## __Example key__
* Client ID / API Key
```
RbvMnSlfD0dRDQ8WDlDEF5cxnvkRlRgf7fuJQBTP5pSd8h8QJv
7fk3hDPqViMBGWbZ3n3fDp1Bekt329ONQyLjvaYXK7iOz7SS6o
XssuwSJuJ3P76sEoW6SK8cBtwdPcTUHAL9yd6oL40SeWkCKUCH
```
* Secret Token
```
fpDXlS9qQaDrWyJyGD4yWNPA2zWo8mk1jLfp4Tu8
LjDeOSRsBeMAfsTEpDxQPbEbu35M3qsNWfD9rsyw
WpwIMbmDPIe60sMF37BHX5JLdldTkMkVhupEcQoF
```
