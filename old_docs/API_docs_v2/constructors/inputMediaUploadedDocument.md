---
title: inputMediaUploadedDocument
description: New document
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: inputMediaUploadedDocument  
[Back to constructors index](index.md)



New document

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|file|[File path or InputFile](../types/InputFile.md) | Yes|The [uploaded file](https://core.telegram.org/api/files)|
|mime\_type|[string](../types/string.md) | Optional|MIME type of document|
|attributes|Array of [DocumentAttribute](../types/DocumentAttribute.md) | Yes|Attributes that specify the type of the document (video, audio, voice, sticker, etc.)|



### Type: [InputMedia](../types/InputMedia.md)


### Example:

```php
$inputMediaUploadedDocument = ['_' => 'inputMediaUploadedDocument', 'file' => InputFile, 'mime_type' => 'string', 'attributes' => [DocumentAttribute, DocumentAttribute]];
```  


Or, if you're into Lua:

```lua
inputMediaUploadedDocument={_='inputMediaUploadedDocument', file=InputFile, mime_type='string', attributes={DocumentAttribute}}

```


