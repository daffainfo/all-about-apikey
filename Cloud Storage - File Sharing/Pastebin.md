# [Pastebin](https://pastebin.com/doc_api)

## __Description__
Plain Text Storage

## __Example Request__
* Curl
```
curl -X POST -d 'api_dev_key={{token}}' -d 'api_paste_code=test' -d 'api_option=paste' "https://pastebin.com/api/api_post.php"
```

* Raw
```
POST /api/api_post.php HTTP/1.1
Host: pastebin.com
Content-Type: application/x-www-form-urlencoded
Content-Length: 81

api_dev_key={{token}}&api_paste_code=test&api_option=paste
```

## __Response__
* Success
```
https://pastebin.com/xxxxxxx
```
* Error
```
Bad API request, invalid api_dev_key
```

## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
5b76f2366bad23eff2f23b781b9389f5
```
 