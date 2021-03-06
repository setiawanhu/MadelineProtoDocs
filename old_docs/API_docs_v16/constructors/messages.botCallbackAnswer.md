---
title: messages.botCallbackAnswer
description: Callback answer sent by the bot in response to a button press
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/constructors/messages_botCallbackAnswer.html
---
# Constructor: messages.botCallbackAnswer  
[Back to constructors index](index.md)



Callback answer sent by the bot in response to a button press

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|alert|[Bool](../types/Bool.md) | Optional|Whether an alert should be shown to the user instead of a toast notification|
|has\_url|[Bool](../types/Bool.md) | Optional|Whether an URL is present|
|message|[string](../types/string.md) | Optional|Alert to show|
|url|[string](../types/string.md) | Optional|URL to open|
|cache\_time|[int](../types/int.md) | Yes|For how long should this answer be cached|



### Type: [messages.BotCallbackAnswer](../types/messages.BotCallbackAnswer.md)


### Example:

```php
$messages.botCallbackAnswer = ['_' => 'messages.botCallbackAnswer', 'alert' => Bool, 'has_url' => Bool, 'message' => 'string', 'url' => 'string', 'cache_time' => int];
```  


Or, if you're into Lua:

```lua
messages.botCallbackAnswer={_='messages.botCallbackAnswer', alert=Bool, has_url=Bool, message='string', url='string', cache_time=int}

```


