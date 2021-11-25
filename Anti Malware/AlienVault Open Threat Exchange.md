# [AlienVault Open Threat Exchange (OTX)](https://otx.alienvault.com/api)

## __Description__
IP/domain/URL reputation

## __Example Request__
* Curl
```
curl https://otx.alienvault.com/api/v1/pulses/subscribed?page=1 \
-H "X-OTX-API-KEY: YOURAPIKEY"
```

* Raw
```
GET /api/v1/pulses/subscribed?page=1 HTTP/1.1
Host: otx.alienvault.com
X-OTX-API-KEY: YOURAPIKEY
```

## __Response__
* Success
```
{
	"results":[
		{
            "id":"60f1357c15569fb2a28d6d8d",
            "name":"Data-Exfiltrator: A New Tactic for Ransomware Adversaries",
            "description":"Ransomware operators have added a specific type of malware to perform this exfiltration to their intrusion set. The malware follows the exfiltration with a single line PowerShell command that stops the malware's .....
    	}
    ]
}
```
* Error
```
{
    "detail": "Authentication required"
} 
```

## __Regex__
```
[a-z0-9]{64}
```

## __Example API key__
```
n71h0x8j6t2j0ta7omdo9c270jahl20mfu0ttz2is1y4neimis7vhwoh1haf1lti
```