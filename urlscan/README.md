# [URLScan](https://urlscan.io/docs/api/)

## __Description__
Scan and Analyse URLs

## __Example Request__
* Curl
```
curl -H "Content-Type: application/json" -H "API-Key: APIKEY" "https://urlscan.io/user/quotas/"
```

* Raw
```
GET /user/quotas/ HTTP/1.1
Host: urlscan.io
Content-Type: application/json
API-Key: APIKEY
```

## __Response__
* Success
```
{
	"source":"user",
	"limits": {
		"private": {
			"day": {
				"limit": 50,
				"used": 0,
				"percent": 0
				}
			//...
```
* Error
```
{
	"message": "API key supplied but not found in database!",
	"status": 401
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
