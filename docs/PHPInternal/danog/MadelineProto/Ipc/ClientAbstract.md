---
title: danog\MadelineProto\Ipc\ClientAbstract: IPC client.
description: 

---
# `danog\MadelineProto\Ipc\ClientAbstract`
[Back to index](../../../index.md)

> Author: Daniil Gentili <daniil@daniil.it>  
  

IPC client.  




## Method list:
* `logger(string $param, int $level, string $file): void`
* `disconnect(): \Generator`

## Methods:
### `logger(string $param, int $level, string $file): void`

Logger.


Parameters:
* `$param`: `string` Parameter  
* `$level`: `int` Logging level  
* `$file`: `string` File where the message originated  



### `disconnect(): \Generator`

Disconnect cleanly from main instance.


Fully typed return value:
```
\Generator<int, \Amp\Promise, mixed, void>
```
#### See also: 
* `\Amp\Promise`
* `\Generator`




---
Generated by [danog/phpdoc](https://phpdoc.daniil.it)
