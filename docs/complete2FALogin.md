---
title: complete_2FA_login
description: complete_2FA_login parameters, return type and example
---
## Method: complete_2FA_login  


### Parameters:

| Name     |    Type       |
|----------|---------------|
|password| A string with the password|

### Return type: [auth.Authorization](API_docs/types/auth_Authorization.md)

### Example ([now fully async!](https://docs.madelineproto.xyz/docs/ASYNC.html)):


```php
yield $MadelineProto->phoneLogin(readline('Enter your phone number: '));
$authorization = yield $MadelineProto->completePhoneLogin(readline('Enter the code you received: '));
if ($authorization['_'] === 'account.noPassword') {
    throw new \danog\MadelineProto\Exception('2FA is enabled but no password is set!');
}
if ($authorization['_'] === 'account.password') {
    $authorization = yield $MadelineProto->complete_2fa_login(readline('Please enter your password (hint '.$authorization['hint'].'): '));
}
if ($authorization['_'] === 'account.needSignup') {
    $authorization = yield $MadelineProto->completeSignup(readline('Please enter your first name: '), readline('Please enter your last name (can be empty): '));
}

```