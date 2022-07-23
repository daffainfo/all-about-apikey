# [Bhagavad Gita](https://docs.bhagavadgitaapi.in/)

## __Description__
Open Source Shrimad Bhagavad Gita API including 21+ authors translation in Sanskrit/English/Hindi

## __Example Request__
* Curl
```
curl https://bhagavadgitaapi.in/slok?api_key={{token}}
```

* Raw
```
GET /slok?api_key={{token}} HTTP/1.1
Host: bhagavadgitaapi.in
```

## __Response__
* Success
```
{
    "_id":"BG17.7",
    "chapter":17,
    "verse":7,
    "slok":"आहारस्त्वपि सर्वस्य त्रिविधो भवति प्रियः |\nयज्ञस्तपस्तथा दानं तेषां भेदमिमं शृणु ||१७-७||",
    "transliteration":"āhārastvapi sarvasya trividho bhavati priyaḥ .\nyajñastapastathā dānaṃ teṣāṃ bhedamimaṃ śṛṇu ||17-7||",
    "tej":{
        "author":"Swami Tejomayananda",
    ...
```
* Error
```
{
    "error":"Invalid api key or given is not provided!"
}
```

## __Regex__
```
[a-z0-9]{17}
```

## __Example API key__
```
id8hnkf8jzgpgf2bv
```