---
title: message
description: A message
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: message  
[Back to constructors index](index.md)



A message

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|unread|[Bool](../types/Bool.md) | Optional|
|out|[Bool](../types/Bool.md) | Optional|Is this an outgoing message|
|mentioned|[Bool](../types/Bool.md) | Optional|Whether we were mentioned in this message|
|media\_unread|[Bool](../types/Bool.md) | Optional|Whether there are unread media attachments in this message|
|id|[int](../types/int.md) | Yes|ID of the message|
|from\_id|[int](../types/int.md) | Optional|ID of the sender of the message|
|to\_id|[Peer](../types/Peer.md) | Yes|ID of the chat were the message was sent|
|fwd\_from\_id|[Peer](../types/Peer.md) | Optional|
|fwd\_date|[int](../types/int.md) | Optional|
|via\_bot\_id|[int](../types/int.md) | Optional|ID of the inline bot that generated the message|
|reply\_to\_msg\_id|[int](../types/int.md) | Optional|ID of the message this message replies to|
|date|[int](../types/int.md) | Yes|Date of the message|
|message|[string](../types/string.md) | Yes|The message|
|media|[MessageMedia](../types/MessageMedia.md) | Optional|Media attachment|
|reply\_markup|[ReplyMarkup](../types/ReplyMarkup.md) | Optional|Reply markup (bot/inline keyboards)|
|entities|Array of [MessageEntity](../types/MessageEntity.md) | Optional|Message [entities](https://core.telegram.org/api/entities) for styled text|
|views|[int](../types/int.md) | Optional|View count for channel posts|



### Type: [Message](../types/Message.md)


### Example:

```php
$message = ['_' => 'message', 'unread' => Bool, 'out' => Bool, 'mentioned' => Bool, 'media_unread' => Bool, 'id' => int, 'from_id' => int, 'to_id' => Peer, 'fwd_from_id' => Peer, 'fwd_date' => int, 'via_bot_id' => int, 'reply_to_msg_id' => int, 'date' => int, 'message' => 'string', 'media' => MessageMedia, 'reply_markup' => ReplyMarkup, 'entities' => [MessageEntity, MessageEntity], 'views' => int];
```  


Or, if you're into Lua:

```lua
message={_='message', unread=Bool, out=Bool, mentioned=Bool, media_unread=Bool, id=int, from_id=int, to_id=Peer, fwd_from_id=Peer, fwd_date=int, via_bot_id=int, reply_to_msg_id=int, date=int, message='string', media=MessageMedia, reply_markup=ReplyMarkup, entities={MessageEntity}, views=int}

```



## Usage of reply_markup

You can provide bot API reply_markup objects here.  


