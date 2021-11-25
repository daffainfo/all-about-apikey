# [Google Safe Browsing](https://developers.google.com/safe-browsing/v4)

## __Description__
Google Link/Domain Flagging

## __Example Request__
* Curl
```
curl --header "Content-Type: application/json" --data "" "https://safebrowsing.googleapis.com/v4/threatListUpdates:fetch?key=API_KEY"
```

* Raw
```
POST /v4/threatListUpdates:fetch?key=API_KEY HTTP/1.1
Host: safebrowsing.googleapis.com
Content-Type: application/json
```

## __Response__
* Success
```
{
	"client": {
    "clientId":       "yourcompanyname",
    "clientVersion":  "1.5.2"
	},
	"listUpdateRequests": [{
		"threatType":      "MALWARE",
		"platformType":    "WINDOWS",
		"threatEntryType": "URL",
		"state":           "Gg4IBBADIgYQgBAiAQEoAQ==",
		"constraints": {
			"maxUpdateEntries":      2048,
			"maxDatabaseEntries":    4096,
			"region":                "US",
			"supportedCompressions": ["RAW"]
			}
		}
	]
}
```
* Error
```
{
    "error": {
        "code": 400,
        "message": "API key not valid. Please pass a valid API key",
        "status": "INVALID_ARGUMENT",                                        "details": [
            {
                "@type": "type.googleapis.com/google.rpc.ErrorInfo",
                "reason": "API_KEY_INVALID","domain": "googleapis.com","metadata": {
                    "service": "safebrowsing.googleapis.com"
                }
            }
        ]
    }
} 
```

## __Regex__
```
AIza[0-9A-Za-z-_]{35}
```

## __Example API key__
```
AIzaSyAtUXpd8JxrpUH2Sd-xO2U_vWGVfoF5-XM
```