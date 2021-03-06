---
title: danog\MadelineProto\SessionPaths: Session path information.
description: 

---
# `danog\MadelineProto\SessionPaths`
[Back to index](../../index.md)

> Author: Daniil Gentili <daniil@daniil.it>  
  

Session path information.  




## Method list:
* `serialize(object $object, string $path): \Generator`
* `unserialize(string $path): \Generator`
* `getLegacySessionPath(): string`
* `getSessionPath(): string`
* `getLockPath(): string`
* `getIpcPath(): string`
* `getIpcStatePath(): string`
* `getIpcState(): \Amp\Promise<?\danog\MadelineProto\Ipc\IpcState>`
* `storeIpcState(): \Generator`
* `getLightStatePath(): string`
* `getLightState(): \Amp\Promise<\danog\MadelineProto\LightState>`
* `storeLightState(): \Generator`
* `getIpcCallbackPath(): string`

## Methods:
### `serialize(object $object, string $path): \Generator`

Serialize object to file.


Parameters:
* `$object`: `object`   
* `$path`: `string`   


#### See also: 
* `\Generator`




### `unserialize(string $path): \Generator`

Deserialize new object.


Parameters:
* `$path`: `string` Object path, defaults to session path  


Fully typed return value:
```
\Generator<mixed, mixed, mixed, object>
```
#### See also: 
* `\Generator`




### `getLegacySessionPath(): string`

Get legacy session path.



### `getSessionPath(): string`

Get session path.



### `getLockPath(): string`

Get lock path.



### `getIpcPath(): string`

Get IPC socket path.



### `getIpcStatePath(): string`

Get IPC light state path.



### `getIpcState(): \Amp\Promise<?\danog\MadelineProto\Ipc\IpcState>`

Get IPC state.


#### See also: 
* [`\danog\MadelineProto\Ipc\IpcState`: IPC state class.](./Ipc/IpcState.md)
* `\Amp\Promise`




### `storeIpcState(): \Generator`

Store IPC state.


#### See also: 
* `\Generator`




### `getLightStatePath(): string`

Get light state path.



### `getLightState(): \Amp\Promise<\danog\MadelineProto\LightState>`

Get light state.


#### See also: 
* `\danog\MadelineProto\LightState`
* `\Amp\Promise`




### `storeLightState(): \Generator`

Store light state.


#### See also: 
* `\Generator`




### `getIpcCallbackPath(): string`

Get IPC callback socket path.



---
Generated by [danog/phpdoc](https://phpdoc.daniil.it)
