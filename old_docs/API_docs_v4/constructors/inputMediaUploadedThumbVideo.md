---
title: inputMediaUploadedThumbVideo
description: inputMediaUploadedThumbVideo attributes, type and example
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: inputMediaUploadedThumbVideo  
[Back to constructors index](index.md)



### Attributes:

| Name     |    Type       | Required |
|----------|---------------|----------|
|file|[File path or InputFile](../types/InputFile.md) | Yes|
|thumb|[File path or InputFile](../types/InputFile.md) | Yes|
|duration|[int](../types/int.md) | Yes|
|w|[int](../types/int.md) | Yes|
|h|[int](../types/int.md) | Yes|
|caption|[string](../types/string.md) | Yes|



### Type: [InputMedia](../types/InputMedia.md)


### Example:

```php
$inputMediaUploadedThumbVideo = ['_' => 'inputMediaUploadedThumbVideo', 'file' => InputFile, 'thumb' => InputFile, 'duration' => int, 'w' => int, 'h' => int, 'caption' => 'string'];
```  


Or, if you're into Lua:

```lua
inputMediaUploadedThumbVideo={_='inputMediaUploadedThumbVideo', file=InputFile, thumb=InputFile, duration=int, w=int, h=int, caption='string'}

```


