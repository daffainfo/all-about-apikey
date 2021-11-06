# [Stytch](https://stytch.com/docs/)

## __Description__
User infrastructure for modern applications

## __Example Request__
* Curl
```
curl --request POST \
	--url https://test.stytch.com/v1/users \
	-u 'PROJECT ID:SECRET' \
	-H 'Content-Type: application/json' \
	-d '{
		"email": "test@stytch.com"
	}'
```

* Raw
```
POST /v1/users HTTP/1.1
Authorization: Basic UFJPSkVDVCBJRDpTRUNSRVQ=
Host: test.stytch.com
Content-Type: application/json
Content-Length: 28

{"email": "test@stytch.com"}
```

## __Response__
* Success

    If the email not exists
```
{
    "email_id":"xxxxxxxxxxxx",
    "phone_id":"",
    "request_id":"xxxxxxxxxxxx",
    "status":"active",
    "status_code":201,
    "user_id":"xxxxxxxxxxxx"
}
```

    If the email exists
```
{
    "status_code":400,
    "request_id":"x","error_type":"duplicate_email",
    "error_message":"A user with the specified email already exists for this project.",
    "error_url":"https://stytch.com/docs/api/errors/400"
}
```
* Error
```
{
    "status_code":401,
    "request_id":"request-id-test-b2001541-53b3-4faa-b7c0-915d2199c9fc",
    "error_type":"unauthorized_credentials",
    "error_message":"Unauthorized credentials.",
    "error_url":"https://stytch.com/docs/api/errors/401"
}
```

## __Regex__
* Project ID
```
project-.*-[a-z0-9]{8}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{4}-[a-z0-9]{12}
```
* Secret Token
```
secret-.*-[a-zA-Z0-9-_=]{36}
```

## __Example key__
* Project ID
```
project-test-c8267d84-db73-5b90-b8c4-e17b456857b8
```
* Secret Token
```
secret-test-wQZjAsRqcO6z-ac1M5t3WfuRy9C_rcFXQ-Y=
secret-test-o1dsqZWeKkX4YSnIspz_LKGjiNFBMMeRJPo=
```
