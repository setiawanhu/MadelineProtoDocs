---
title: messages.stickers
description: Found stickers
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/constructors/messages_stickers.html
---
# Constructor: messages.stickers  
[Back to constructors index](index.md)



Found stickers

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|hash|[string](../types/string.md) | Yes|Hash|
|stickers|Array of [Document](../types/Document.md) | Yes|Stickers|



### Type: [messages.Stickers](../types/messages.Stickers.md)


### Example:

```php
$messages.stickers = ['_' => 'messages.stickers', 'hash' => 'string', 'stickers' => [Document, Document]];
```  


Or, if you're into Lua:

```lua
messages.stickers={_='messages.stickers', hash='string', stickers={Document}}

```


