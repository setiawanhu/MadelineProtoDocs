---
title: messages.getInlineBotResults
description: Query an inline bot
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/messages_getInlineBotResults.html
---
# Method: messages.getInlineBotResults
[Back to methods index](index.md)



Query an inline bot

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|bot|[Username, chat ID, Update, Message or InputUser](../types/InputUser.md) | The bot to query | Optional|
|query|[string](../types/string.md) | The query | Yes|
|offset|[string](../types/string.md) | The offset within the results, will be passed directly as-is to the bot. | Yes|


### Return type: [messages.BotResults](../types/messages.BotResults.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$messages.BotResults = $MadelineProto->messages->getInlineBotResults(['bot' => InputUser, 'query' => 'string', 'offset' => 'string', ]);
```

Or, if you're into Lua:

```lua
messages.BotResults = messages.getInlineBotResults({bot=InputUser, query='string', offset='string', })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|BOT_INLINE_DISABLED|This bot can't be used in inline mode|
|400|BOT_INVALID|This is not a valid bot|
|400|BOT_RESPONSE_TIMEOUT|A timeout occurred while fetching data from the bot|
|400|CHANNEL_PRIVATE|You haven't joined this channel/supergroup|
|400|INPUT_USER_DEACTIVATED|The specified user was deleted|
|400|MSG_ID_INVALID|Invalid message ID provided|
|-503|Timeout|Timeout while fetching data|


