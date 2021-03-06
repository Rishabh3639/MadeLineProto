---
title: updates.getState
description: updates.getState parameters, return type and example
---
## Method: updates.getState  
[Back to methods index](index.md)


*You cannot use this method directly, see https://daniil.it/MadelineProto for more info on handling updates*






### Return type: [updates\_State](../types/updates_State.md)

### Example:


```
$MadelineProto = new \danog\MadelineProto\API();
if (isset($token)) { // Login as a bot
    $MadelineProto->bot_login($token);
}
if (isset($number)) { // Login as a user
    $sentCode = $MadelineProto->phone_login($number);
    echo 'Enter the code you received: ';
    $code = '';
    for ($x = 0; $x < $sentCode['type']['length']; $x++) {
        $code .= fgetc(STDIN);
    }
    $MadelineProto->complete_phone_login($code);
}

$updates_State = $MadelineProto->updates->getState();
```

Or, if you're using the [PWRTelegram HTTP API](https://pwrtelegram.xyz):

### As a bot:

POST/GET to `https://api.pwrtelegram.xyz/botTOKEN/madeline`

Parameters:

* method - updates.getState
* params - `{}`



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/updates.getState`

Parameters:




Or, if you're into Lua:

```
updates_State = updates.getState({})
```

