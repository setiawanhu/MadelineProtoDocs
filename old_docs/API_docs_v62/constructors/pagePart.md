---
title: pagePart
description: Page part
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: pagePart  
[Back to constructors index](index.md)



Page part

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|blocks|Array of [PageBlock](../types/PageBlock.md) | Yes|Blocks|
|photos|Array of [Photo](../types/Photo.md) | Yes|Photos|
|videos|Array of [Document](../types/Document.md) | Yes|Videos|



### Type: [Page](../types/Page.md)


### Example:

```php
$pagePart = ['_' => 'pagePart', 'blocks' => [PageBlock, PageBlock], 'photos' => [Photo, Photo], 'videos' => [Document, Document]];
```  


Or, if you're into Lua:

```lua
pagePart={_='pagePart', blocks={PageBlock}, photos={Photo}, videos={Document}}

```


