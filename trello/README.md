# [Trello](https://developers.trello.com/)

## __Description__
Boards, lists and cards to help you organize and prioritize your projects

## __Example Request__
* Curl
```
curl "https://trello.com/1/authorize?expiration=never&scope=read,write,account&response_type=token&name=Server%20Token&key={{token}}"
```

* Raw
```
GET /1/authorize?expiration=never&scope=read,write,account&response_type=token&name=Server%20Token&key={{token}} HTTP/1.1
Host: trello.com
```

## __Response__
* Success
```
<!DOCTYPE html>

<html lang="en">
<head>                                                                                                           
...
</head>
<script>
...
</script>
<body class="account-page request-token" onload="setup();"> 
    <div class="account-header compact">
        <img alt="Trello logo" src="/images/trello-logo-blue.svg">
    </div>
    <div id="surface">
        <div class="account-content clearfix">
            <div class="authorization-question">
                <h1>Would you like to give the following application access to your account?</h1>
            </div>
        <hr>
        ...
```
* Error
```
App not found
```

## __Regex__
```
[0-9a-z]{32}
```

## __Example API key__
```
bb1aa18d0eeea0fc7ggg799h3i9578j
```