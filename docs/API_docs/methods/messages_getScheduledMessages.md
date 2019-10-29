---
title: messages.getScheduledMessages
description: Get scheduled messages
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Method: messages.getScheduledMessages  
[Back to methods index](index.md)


Get scheduled messages

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|peer|[Username, chat ID, Update, Message or InputPeer](../types/InputPeer.md) | Peer | Optional|
|id|Array of [int](../types/int.md) | ID | Yes|


### Return type: [messages\_Messages](../types/messages_Messages.md)

### Can bots use this method: **YES**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$messages_Messages = $MadelineProto->messages->getScheduledMessages(['peer' => InputPeer, 'id' => [int, int], ]);
```

Or, if you're into Lua:

```lua
messages_Messages = messages.getScheduledMessages({peer=InputPeer, id={int}, })
```
