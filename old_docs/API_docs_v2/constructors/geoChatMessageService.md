---
title: geoChatMessageService
description: geoChatMessageService attributes, type and example
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: geoChatMessageService  
[Back to constructors index](index.md)



### Attributes:

| Name     |    Type       | Required |
|----------|---------------|----------|
|chat\_id|[int](../types/int.md) | Yes|
|id|[int](../types/int.md) | Yes|
|from\_id|[int](../types/int.md) | Yes|
|date|[int](../types/int.md) | Yes|
|action|[MessageAction](../types/MessageAction.md) | Optional|



### Type: [GeoChatMessage](../types/GeoChatMessage.md)


### Example:

```php
$geoChatMessageService = ['_' => 'geoChatMessageService', 'chat_id' => int, 'id' => int, 'from_id' => int, 'date' => int, 'action' => MessageAction];
```  


Or, if you're into Lua:

```lua
geoChatMessageService={_='geoChatMessageService', chat_id=int, id=int, from_id=int, date=int, action=MessageAction}

```


