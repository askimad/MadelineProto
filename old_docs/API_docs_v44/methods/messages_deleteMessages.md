---
title: messages.deleteMessages
description: Delete messages
---
## Method: messages.deleteMessages  
[Back to methods index](index.md)


Delete messages

### Parameters:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|id|Array of [CLICK ME int](../types/int.md) | Yes|IDs of messages to delete, use channels->deleteMessages for supergroups|


### Return type: [messages\_AffectedMessages](../types/messages_AffectedMessages.md)

### Can bots use this method: **YES**


### Errors this method can return:

| Error    | Description   |
|----------|---------------|
|MESSAGE_DELETE_FORBIDDEN|You can't delete one of the messages you tried to delete, most likely because it is a service message.|


### MadelineProto Example:


```
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$messages_AffectedMessages = $MadelineProto->messages->deleteMessages(['id' => [int, int], ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):

### As a bot:

POST/GET to `https://api.pwrtelegram.xyz/botTOKEN/madeline`

Parameters:

* method - messages.deleteMessages
* params - `{"id": [int], }`



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/messages.deleteMessages`

Parameters:

id - Json encoded  array of int




Or, if you're into Lua:

```
messages_AffectedMessages = messages.deleteMessages({id={int}, })
```

