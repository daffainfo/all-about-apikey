# [ExchangeRate-API](https://www.exchangerate-api.com/docs/overview)

## __Description__
Free currency conversion

## __Example Request__
* Curl
```
curl "https://v6.exchangerate-api.com/v6/{{token}}/latest/USD"
```

* Raw
```
GET /v6/{{token}}/latest/USD HTTP/1.1
Host: v6.exchangerate-api.com
```

## __Response__
* Success
```
{
	"result": "success",
	"documentation": "https://www.exchangerate-api.com/docs",
	"terms_of_use": "https://www.exchangerate-api.com/terms",
	"time_last_update_unix": 1585267200,
	"time_last_update_utc": "Fri, 27 Mar 2020 00:00:00 +0000",
	"time_next_update_unix": 1585353700,
	"time_next_update_utc": "Sat, 28 Mar 2020 00:00:00 +0000",
	"base_code": "USD",
	"conversion_rates": {
		"USD": 1,
		"AUD": 1.4817,
		"BGN": 1.7741,
		"CAD": 1.3168,
		"CHF": 0.9774,
		"CNY": 6.9454,
        ...
	}
}
```
* Error
```
{
    "result":"error",
    "documentation":"https://www.exchangerate-api.com/docs",
    "terms-of-use":"https://www.exchangerate-api.com/terms",
    "error-type":"invalid-key"
}
```
## __Regex__
```
[a-z0-9]{24}
```

## __Example API key__
```
0bba3f2c5f3083ba3623938d
```
