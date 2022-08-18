# [Cloudmersive](https://api.cloudmersive.com/)

## __Description__
A Utility API platform provides layers of API coverage, allowing businesses to accelerate both project and deliverable completion times, as well as increase information security and standardize organizational output across working groups and teams.

## __Example Request__
* Curl
```
curl --location --request POST "https://api.cloudmersive.com/barcode/lookup/ean" --header "Content-Type: application/x-www-form-urlencoded" --header "Apikey: {{token}}" -d "0=<&1=s&2=t&3=r&4=i&5=n&6=g&7=>"
```

* Raw
```
POST /barcode/lookup/ean HTTP/1.1
Host: api.cloudmersive.com
Content-Type: application/x-www-form-urlencoded
Apikey: {{token}}
Content-Length: 31

0=<&1=s&2=t&3=r&4=i&5=n&6=g&7=>
```

## __Response__
* Success
```
{
    "Successful":true,
    "Matches":[]
}
```
* Error
```
401 Invalid API key or exceeded limits.
```
## __Regex__
```
[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}
```

## __Example API key__
```
abcd1234-abcd-1234-abcd-abcd1234abcd
```