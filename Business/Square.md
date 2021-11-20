# [Square](https://developer.squareup.com/reference/square)

## __Description__
Easy way to take payments, manage refunds, and help customers checkout online

## __Example Request__
* Curl
```
curl https://connect.squareupsandbox.com/v2/payments -H "Authorization: Bearer {{token}}"
```

* Raw
```
GET /v2/payments HTTP/1.1
Authorization: Bearer {{token}}
Host: connect.squareupsandbox.com
```

## __Response__
* Success
```
{}
```
* Error
```
{
    "errors": [
        {
            "code": "UNAUTHORIZED",
            "detail": "The `Authorization` http header of your request was incorrect or expired. The header value is expected to be of the format \"Bearer TOKEN\" (without quotation marks), where TOKEN is a valid access token (e.g. \"Bearer ABC123def456GHI789jkl0\"). For more information, see https://developer.squareup.com/docs/build-basics/using-rest-api#__set-the-headers__ .",
            "category": "AUTHENTICATION_ERROR"
        }
    ]
}
```

## __Regex__
```
EAAAE[a-zA-Z0-9_-]{59}
```

## __Example API key__
```
EAAAEKR1-pYM45dOv-uDpcJO06g5kGjwqlaT3YK3vxY5xNr66gJxdiG2pzW5lEm-
EAAAEEW9SGAolaA3gTPc30nZSoyssNPJjn3oiKsKQR_JUxix93yi0rW6RfxUqkFG
```