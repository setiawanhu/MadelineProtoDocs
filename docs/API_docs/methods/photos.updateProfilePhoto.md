---
title: photos.updateProfilePhoto
description: Installs a previously uploaded photo as a profile photo.
image: https://docs.madelineproto.xyz/favicons/android-chrome-256x256.png
redirect_from: /API_docs/methods/photos_updateProfilePhoto.html
---
# Method: photos.updateProfilePhoto
[Back to methods index](index.md)



Installs a previously uploaded photo as a profile photo.

### Parameters:

| Name     |    Type       | Description | Required |
|----------|---------------|-------------|----------|
|id|[MessageMedia, Update, Message or InputPhoto](../types/InputPhoto.md) | Input photo | Optional|


### Return type: [photos.Photo](../types/photos.Photo.md)

### Can bots use this method: **NO**


### MadelineProto Example ([now async for huge speed and parallelism!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$photos.Photo = $MadelineProto->photos->updateProfilePhoto(['id' => InputPhoto, ]);
```

Or, if you're into Lua:

```lua
photos.Photo = photos.updateProfilePhoto({id=InputPhoto, })
```

### Errors

| Code | Type     | Description   |
|------|----------|---------------|
|400|FILE_PARTS_INVALID|The number of file parts is invalid|
|400|IMAGE_PROCESS_FAILED|Failure while processing image|
|400|LOCATION_INVALID|The provided location is invalid|
|400|PHOTO_CROP_SIZE_SMALL|Photo is too small|
|400|PHOTO_EXT_INVALID|The extension of the photo is invalid|
|406|AUTH_KEY_DUPLICATED|An auth key with the same ID was already generated|


