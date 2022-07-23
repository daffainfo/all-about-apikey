# [Lob](https://docs.lob.com/)

## __Description__
US Address Verification

## __Example Request__
* Curl
```
curl https://api.lob.com/v1/addresses -u {{token}}:
```

* Raw
```
GET /v1/addresses HTTP/1.1
Authorization: Basic dGVzdF8wZGM4ZDUxZTBhY2ZmY2IxODgwZTBmMTljNzliMmY1YjBjYzo=
Host: api.lob.com
```

## __Response__
* Success
```
{
    "data": [
        {
            "id": "adr_5e578da6464949d0",
            "description": null,
            "name": "JOHN DOE",
            "company": null,
            "phone": null,
            "email": null,
            "address_line1": "123 MAIN ST",
            "address_line2": null,
            "address_city": "SAN FRANCISCO",
            "address_state": "CA",
            "address_zip": "94105-1804",
            "address_country": "UNITED STATES",
            "metadata": {},
            "date_created": "2022-06-15T19:37:36.835Z",
            "date_modified": "2022-06-15T19:37:36.835Z",
            "object": "address"
        },
```
* Error
```
{
    "error": {
        "message": "Your API key is not valid. Please sign up on lob.com to get a valid api key.",
        "status_code": 401,
        "code": "invalid_api_key"
    }
}
```
## __Regex__
```
test_[a-z0-9]{35}
```

## __Example API key__
```
test_0dc8d51e0acffcb1880eabf9283sop5b0cc
```
