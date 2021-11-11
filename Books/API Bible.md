# [API Bible](https://docs.api.bible/)

## __Description__
Everything you need from the Bible in one discoverable place

## __Example Request__
* Curl
```
curl -s -H "api-key: YOURAPIKEY" https://api.scripture.api.bible/v1/bibles/a6aee10bb058511c-02/verses/JHN.3.16\?fums-version\=3
```

* Raw
```
GET /v1/bibles/a6aee10bb058511c-02/verses/JHN.3.16?fums-version=3 HTTP/1.1
Host: api.scripture.api.bible
api-key: YOURAPIKEY
```

## __Response__
* Success
```
{
  "data": {
    "id": "JHN.3.16",
    "orgId": "JHN.3.16",
    "bookId": "JHN",
    "chapterId": "JHN.3",
    "bibleId": "a6aee10bb058511c-02",
    "reference": "John 3:16",
    "content": "<p class=\"s1\">God So Loved the World</p><p class=\"p\"><span data-number=\"16\" class=\"v\">16</span>For God so loved the world, that he gave his only begotten Son, that whosoever believeth in him should not perish, but have everlasting life. </p>",
    "verseCount": 1,
    "copyright": "King James Version 1611, spelling, punctuation and text formatting modernized by ABS in 1962; typesetting © 2010 American Bible Society.",
    "next": {
      "id": "JHN.3.17",
      "number": "17"
    },
    "previous": {
      "id": "JHN.3.15",
      "number": "15"
    }
  },
  "meta": {
    "fumsToken": "G0wBgBwHbqxlyoOgvZ6lYyp_uvBQFmocvykgSJauvtB528beKuJyHB2OZq8VtIOgO2u2mhHYxiiJ0fzDzeUfz9sB8C_21Fze_TRNl0um2YxiicxzS-KVgtSu1xk5dZwAzX8QIoPp5dJdgAPVxKnEmlM0oCDhj8lYMUM4wCkvEQPBBjxyYVksCbunKC0UV2oZA7Z3ufLztgQ1fftYcvRhYtohRHILNlg9j_ezKk416zSv2p8WcWlDyWTLYjq3S50XSiuaLapg"
  }
}
```
* Error
```
{
    "statusCode":401,
    "error":"Unauthorized",
    "message":"missing key"
}
```

## __Regex__
```
[a-z0-9]{32}
```

## __Example API key__
```
mrid9uaaildwnsbukhzdqA2ya1u9shld
```