# [Dribbble](https://developer.dribbble.com/v2/)

## __Description__
Dribbble is a self-promotion and social networking platform for digital designers and creatives

## __Example Request__
* Curl
```
curl "https://api.dribbble.com/v2/user?access_token=ACCESS_TOKEN"
```

* Raw
```
GET /v2/user?access_token=ACCESS_TOKEN HTTP/1.1
Host: api.dribbble.com
```

## __Response__
* Success
```
{
    "id" : 1,
    "name" : "Dan Cederholm",
    "login" : "simplebits",
    "html_url" : "https://dribbble.com/simplebits",
    "avatar_url" : "https://d13yacurqjgara.cloudfront.net/users/1/avatars/normal/dc.jpg?1371679243",
    "bio" : "Co-founder &amp; designer of <a href=\"https://dribbble.com/dribbble\">@Dribbble</a>. Principal of SimpleBits. Aspiring clawhammer banjoist.",
    "location" : "Salem, MA",
    ....
```
* Error
```
{
    "message":"Bad credentials."
}
```

## __Regex__
```
[a-z0-9]{64}
```

## __Example API key__
```
om34l6c32snpjr1tsj7fixoexafrgr9i6023t2701yysa7fuqfbdgy0tct75gkeg
```