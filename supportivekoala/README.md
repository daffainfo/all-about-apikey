# [Supportivekoala](https://developers.supportivekoala.com/)

## __Description__
Autogenerate images with template

## __Example Request__
* Curl
```
curl --location --request GET "https://api.supportivekoala.com/v1/images" --header "Content-Type: application/json" --header "Authorization: Bearer {{token}}"
```

* Raw
```
GET /v1/images HTTP/1.1
Host: api.supportivekoala.com
Content-Type: application/json
Authorization: Bearer {{token}}
```

## __Response__
* Success
```
[
    {
        "_id": "61158cbcb18087773138fc55",
        "template": "61ce63fe5bbbc920d0038182",
        "imageUrl": "https://cloud.supportivekoala.com/3361663f-d1fd-4a26-a1aa-75aa155e5fa7.png",
        "createdAt": "2021-08-12T21:03:56.769Z",
        "updatedAt": "2021-08-12T21:03:56.769Z",
        "__v": 0
    }
]
```
* Error
```
{
    "code":401,
    "message":"invalid signature"
}
```
## __Regex__
```
^[A-Za-z0-9-_=]+\.[A-Za-z0-9-_=]+\.?[A-Za-z0-9-_.+/=]*$
```

## __Example API key__
```
eyJpc3MiOiJPbmxpbmUgSldUIEJ1aWxkZXIiLCJpYXQiOjE2M.jkxMDcxMjAsImV4cCI6MTY2MDY0MzEyMCwiYXVkIjo........
```
