---
title: account.getContentSettings
description: account.getContentSettings parameters, return type and example
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/account_getContentSettings.html
---
# Method: account.getContentSettings  
[Back to methods index](index.md)




### Return type: [account.ContentSettings](../types/account.ContentSettings.md)

### Can bots use this method: **YES**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$account.ContentSettings = $MadelineProto->account->getContentSettings();
```

Or, if you're into Lua:

```lua
account.ContentSettings = account.getContentSettings({})
```

