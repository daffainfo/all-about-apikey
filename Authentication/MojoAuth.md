# [MojoAuth](https://mojoauth.com/)

## __Description__
Secure and modern passwordless authentication platform

## __Example Request__
* Curl
```
curl -X POST -H "X-API-Key: YOURAPIKEY" https://api.mojoauth.com/token/jwks
```

* Raw
```
POST /token/jwks HTTP/1.1
Host: api.mojoauth.com
X-API-Key: YOURAPIKEY
```

## __Response__
* Success
```
{
    "keys": [{
        "kty": "RSA",
        "kid": "xxxxxxxxxxxxxx",
        "use": "sig",
        "alg": "RS256",
        "n": "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
        "e": "XXXX"
    }]
}
```
* Error
```
{
    "code": 905,
    "message": "API key is invalid",
    "description": "The provided API key is invalid, please use a valid API key of your MojoAuth account."
}
```

## __Regex__
```
[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}
```

## __Example API key__
```
c8267d84-db73-5b90-b8c4-e17b456857b8
```