# [Word Cloud](https://wordcloudapi.com/)

## __Description__
Easily create word clouds

## __Example Request__
* Curl
```
curl -X POST --header "content-type: application/json" -H "x-rapidapi-host: textvis-word-cloud-v1.p.rapidapi.com" -H "x-rapidapi-key: YOURAPIKEY" "https://textvis-word-cloud-v1.p.rapidapi.com/v1/textToCloud" --data '{
  "text": "This is a test. I repeat, this is a test. We are only testing the functionality of this api, nothing else. End of test.",
  "scale": 0.5,
  "width": 400,
  "height": 400,
  "colors": [
    "#375E97",
    "#FB6542",
    "#FFBB00",
    "#3F681C"
  ],
  "font": "Tahoma",
  "use_stopwords": true,
  "language": "en",
  "uppercase": false
}'
```

* Raw
```
POST /v1/textToCloud HTTP/1.1
Host: textvis-word-cloud-v1.p.rapidapi.com
content-type: application/json
x-rapidapi-host: textvis-word-cloud-v1.p.rapidapi.com
x-rapidapi-key: YOURAPIKEY
Content-Length: 349

{
  "text": "This is a test. I repeat, this is a test. We are only testing the functionality of this api, nothing else. End of test.",
  "scale": 0.5,
  "width": 400,
  "height": 400,
  "colors": [
    "#375E97",
    "#FB6542",
    "#FFBB00",
    "#3F681C"
  ],
  "font": "Tahoma",
  "use_stopwords": true,
  "language": "en",
  "uppercase": false
}
```

## __Response__
* Success
```
*The website will return base64 image
```
* Error
```
{
    "message": "You are not subscribed to this API."
}
```

## __Regex__
```
[a-z0-9]{50}
```

## __Example API key__
```
kks6qgj47efs2v1i9cv8b7q2in0hs5088o4r9u4ce6h3xjvnmj
```