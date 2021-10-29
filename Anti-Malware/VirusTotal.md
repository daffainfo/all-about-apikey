# [VirusTotal](https://developers.virustotal.com/reference#getting-started)

## __Description__
VirusTotal File/URL Analysis

## __Example Request__
* Curl
```
curl --request POST --url "https://www.virustotal.com/vtapi/v2/url/scan" -d "apikey=APIKEY" --data "url=google.com"
```

* Raw
```
POST /vtapi/v2/url/scan HTTP/1.1
Host: www.virustotal.com
Content-Type: application/x-www-form-urlencoded
Content-Length: 86

apikey=APIKEY&url=google.com
```

## __Response__
* Success
```
{
	"permalink": "https://www.virustotal.com/gui/url/xxxxxx/detection/u-xxxxxxxxxxx-111111111",
	"resource": "http://google.com/",
	"url": "http://google.com/",
	"response_code": 1,
	"scan_date": "2021-08-16 05:56:27",
	"scan_id": "xxxxxxx-11111111",
	"verbose_msg": "Scan request successfully queued, come back later for the report"
}
```
* Error
```

```
>Blank response if error

## __Regex__
```
[a-z0-9]{64}
```

## __Example API key__
```
w5kukcma7yfj8m8p5rkjx5chg3nno9z7h7wr4o8uq1n0pmr5dfejox4oz4xr7g3c
```