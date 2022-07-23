# [AdoptAPet](https://www.adoptapet.com/public/apis/pet_list.html)

## __Description__
Resource to help get pets adopted

## __Example Request__
* Curl
```
curl "https://api.adoptapet.com/search/pets_at_shelter?key=YOURAPIKEY&v=2&output=json&shelter_id=79570&start_number=1&end_number=500"
```

* Raw
```
GET /search/pets_at_shelter?key=YOURAPIKEY&v=2&output=json&shelter_id=79570&start_number=1&end_number=500 HTTP/1.1
Host: api.adoptapet.com
```

## __Response__
* Success
```
{
    "returned_pets":1,
    "total_pets":1,
    "pets":[
        {
            "age":"adult",
            "secondary_breed":null,
            "large_results_photo_width":200,
            "species":"dog",
            "sex":"m",
            "addr_state_code":"TX",
            ...
        }
    ],
    "status":"ok"
}
```
* Error
```
{
    "error":{
        "code":401,
        "msg":"invalid_key"
    },
    "status":"fail"
}
```

## __Regex__
```
[a-z0-9]{33}
```

## __Example API key__
```
atkynd0qgc6a6eo2zgmm3jpjuuyi1s4w1
```