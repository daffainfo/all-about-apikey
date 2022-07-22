# [CodeStats](https://codestats.net/api-docs)

## __Description__
Automatic time tracking for programmers

## __Example Request__
* Curl
```
curl -XPOST "https://codestats.net/api/my/pulses" -H "X-API-Token: {{token}}" -d '{"coded_at": "2016-04-24T01:43:56+12:00","xps": [{"language": "C++","xp": 15},{"language": "Elixir", "xp": 30},{"language": "EEx","xp": 3}]}'
```

* Raw
```
POST /api/my/pulses HTTP/1.1
Host: codestats.net
X-API-Token: {{token}}
Content-Length: 140

{
  "coded_at": "2016-04-24T01:43:56+12:00",
  "xps": [
    {"language": "C++",    "xp": 15},
    {"language": "Elixir", "xp": 30},
    {"language": "EEx",    "xp": 3}
  ]
}
```

## __Response__
* Success
```
{
    "ok": "Great success!"
}
```
* Error
```
{
    "error": "You must be authenticated"
}
```
## __Regex__
```
SFMyNTY\.[A-Za-z0-9-_=]+\.?[A-Za-z0-9-_.+/=]*$
```

## __Example API key__
```
SFMyNTY.OEotWWdnPT0jI01qaz0.X0wVEZquh8Ogau1iTtBihYqqL71FD8N6p5ChQiIpaxQ....
```