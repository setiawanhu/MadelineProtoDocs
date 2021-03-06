---
title: account.registerDevice
description: Register device to receive [PUSH notifications](https://core.telegram.org/api/push-updates)
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/account_registerDevice.html
---
# Method: account.registerDevice  
[Back to methods index](index.md)


Register device to receive [PUSH notifications](https://core.telegram.org/api/push-updates)

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|token\_type|[int](../types/int.md) | Device token type.<br>**Possible values**:<br>`1` \- APNS (device token for apple push)<br>`2` \- FCM (firebase token for google firebase)<br>`3` \- MPNS (channel URI for microsoft push)<br>`4` \- Simple push (endpoint for firefox's simple push API)<br>`5` \- Ubuntu phone (token for ubuntu push)<br>`6` \- Blackberry (token for blackberry push)<br>`7` \- Unused<br>`8` \- WNS (windows push)<br>`9` \- APNS VoIP (token for apple push VoIP)<br>`10` \- Web push (web push, see below)<br>`11` \- MPNS VoIP (token for microsoft push VoIP)<br>`12` \- Tizen (token for tizen push)<br><br>For `10` web push, the token must be a JSON-encoded object containing the keys described in [PUSH updates](https://core.telegram.org/api/push-updates) | Yes|
|token|[string](../types/string.md) | Device token | Yes|
|device\_model|[string](../types/string.md) | Device model | Yes|
|system\_version|[string](../types/string.md) | System version | Yes|
|app\_version|[string](../types/string.md) | App version | Yes|
|app\_sandbox|[Bool](../types/Bool.md) | If [(boolTrue)](../constructors/boolTrue.md) is transmitted, a sandbox-certificate will be used during transmission. | Yes|
|lang\_code|[string](../types/string.md) | Language code | Yes|


### Return type: [Bool](../types/Bool.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$Bool = $MadelineProto->account->registerDevice(['token_type' => int, 'token' => 'string', 'device_model' => 'string', 'system_version' => 'string', 'app_version' => 'string', 'app_sandbox' => Bool, 'lang_code' => 'string', ]);
```

Or, if you're into Lua:

```lua
Bool = account.registerDevice({token_type=int, token='string', device_model='string', system_version='string', app_version='string', app_sandbox=Bool, lang_code='string', })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|TOKEN_INVALID|The provided token is invalid|


