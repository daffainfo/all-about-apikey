# [ORB Intelligence](https://api.orb-intelligence.com/docs/)

## __Description__
Company lookup

## __Example Request__
* Curl
```
curl -X GET --header "Accept: application/json" "https://api.orb-intelligence.com/3/fetch/1/?api_key={{token}}"
```

* Raw
```
GET /3/fetch/1/?api_key={{token}} HTTP/1.1
Host: api.orb-intelligence.com
Accept: application/json
```

## __Response__
* Success
```
{
    "entity_type": "company",
    "company_status": "active",
    "orb_num": 1,
    "orb_nums": [1],
    "parent_orb_num": null,
    "parent_name": null,
    "branches_count": 0,
    "subsidiaries_count": 0,
    "ultimate_parent_orb_num": null,
    "ultimate_parent_name": null,
    ...
```
* Error
```
API key is invalid or expired.
```

## __Regex__
```
[a-f0-9]{8}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{4}-[a-f0-9]{12}
```

## __Example API key__
```
c8267d84-db73-5b90-b8c4-e17b456857b8
```