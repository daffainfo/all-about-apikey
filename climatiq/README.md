# [Climatiq](https://docs.climatiq.io/)

## __Description__
Calculate the environmental footprint created by a broad range of emission-generating activities

## __Example Request__
* Curl
```
curl "https://beta3.api.climatiq.io/search?query=light+duty+trucks&year=2021" -H "Authorization: Bearer {{token}}"
```

* Raw
```
GET /search?query=light+duty+trucks&year=2021 HTTP/1.1
Host: beta3.api.climatiq.io
Authorization: Bearer {{token}}
```

## __Response__
* Success
```
{
    "current_page": 1,
    "last_page": 11,
    "total_results": 218,
    "results": [
        {
        "activity_id": "commercial_vehicle-vehicle_type_truck_light-fuel_source_na-engine_size_na-vehicle_age_na-vehicle_weight_na",
        "uuid": "05d034db-dfe7-462e-9a19-a69ecd65a114",
        "id": "commercial_vehicle-vehicle_type_truck_light-fuel_source_na-engine_size_na-vehicle_age_na-vehicle_weight_na",
        "name": "Light-Duty Truck",
        "category": "Vehicles",
        ...
```
* Error
```
{
    "error": "unauthorized",
    "message": "Your authentication token was not valid"
}
```
## __Regex__
```
[A-Z0-9]{28}
```

## __Example API key__
```
V9NPRSZ3KF4XN4Q8G50J3Y1DXRVQ
```