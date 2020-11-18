---
title: danog\MadelineProto\MTProtoSession\MsgIdHandler: Manages message ids.
description: 

---
# `danog\MadelineProto\MTProtoSession\MsgIdHandler`
[Back to index](../../../index.md)

> Author: Daniil Gentili <daniil@daniil.it>  
  

Manages message ids.  




## Method list:
* `createInstance(\danog\MadelineProto\Connection $session): self`
* `checkMessageId(string $newMessageId, array $aargs): void`
* `generateMessageId(): string`
* `getMaxId(bool $incoming): mixed`
* `toString(string $messageId): string`

## Methods:
### `createInstance(\danog\MadelineProto\Connection $session): self`

Create MsgIdHandler instance.


Parameters:
* `$session`: `\danog\MadelineProto\Connection` Session  


#### See also: 
* `\danog\MadelineProto\Connection`




### `checkMessageId(string $newMessageId, array $aargs): void`

Check validity of given message ID.


Parameters:
* `$newMessageId`: `string` New message ID  
* `$aargs`: `array` Params  



### `generateMessageId(): string`

Generate outgoing message ID.



### `getMaxId(bool $incoming): mixed`

Get maximum message ID.


Parameters:
* `$incoming`: `bool` Incoming or outgoing message ID  



### `toString(string $messageId): string`

Get readable representation of message ID.


Parameters:
* `$messageId`: `string`   



---
Generated by [danog/phpdoc](https://phpdoc.daniil.it)