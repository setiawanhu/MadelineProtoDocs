---
title: pageBlockRelatedArticles
description: Related articles
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
---
# Constructor: pageBlockRelatedArticles  
[Back to constructors index](index.md)



Related articles

### Attributes:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|title|[RichText](../types/RichText.md) | Yes|Title|
|articles|Array of [PageRelatedArticle](../types/PageRelatedArticle.md) | Yes|Related articles|



### Type: [PageBlock](../types/PageBlock.md)


### Example:

```php
$pageBlockRelatedArticles = ['_' => 'pageBlockRelatedArticles', 'title' => RichText, 'articles' => [PageRelatedArticle, PageRelatedArticle]];
```  


Or, if you're into Lua:

```lua
pageBlockRelatedArticles={_='pageBlockRelatedArticles', title=RichText, articles={PageRelatedArticle}}

```


