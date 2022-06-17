# [OpenAPIHub](https://hub.openapihub.com/en-us/api-catalogue/All)

## __Description__
The All-in-one API Platform

## __Example Request__

For the URL, it depends on the API, for example I am using [Credit Card Number Generator](https://hub.openapihub.com/en-us/v/dev-geeks-7gz88/api/credit-card-number-generator-s9s6b/readme)

* Curl
```
curl "https://trial-api-credit-card-number-generator-2m83.gw.openapihub.com/random_card_number?vendor=visa" -H "X-OpenAPIHub-Key: {{token}}"
```

* Raw
```
GET /random_card_number?vendor=visa HTTP/1.1
Host: trial-api-credit-card-number-generator-2m83.gw.openapihub.com
X-OpenAPIHub-Key: {{token}}
```

## __Response__
* Success
```
{
    "number": "3577359805860126",
    "vendor": "jcb"
}
```
* Error
```
{
    "message":"Invalid authentication credentials"
}
```
## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
tue3sv9hzsey1me4l7fwq3t46u5k8wag
```
