# [Wordnik](https://developer.wordnik.com/docs)

## __Description__
Dictionary Data

## __Example Request__
* Curl
```
curl "https://api.wordnik.com/v4/word.json/hedgehog/topExample?useCanonical=false&api_key={{token}}"
```

* Raw
```
GET /v4/word.json/hedgehog/topExample?useCanonical=false&api_key={{token}} HTTP/1.1
Host: api.wordnik.com
```

## __Response__
* Success
```
{
    "provider": {
        "id":711
    },
    "year":1883,
    "rating":430.02264,
    "url":"http://digital.library.upenn.edu/women/carlyle/jwclam/lam.html",
    "word":"hedgehog",
    "text":"Last night, however, I bought a - hedgehog from a wee boy.",
    "documentId":30111425,
    "exampleId":1097914105,
    "title":"Letters and Memorials of Jane Welsh Carlyle"
}
```
* Error
```
{
    "message":"Invalid authentication credentials"
}
```
## __Regex__
```
[a-z0-9]{49}
```

## __Example API key__
```
ac6099e63826b8650f05ac6099e63826b8650f05668e3f161
```
