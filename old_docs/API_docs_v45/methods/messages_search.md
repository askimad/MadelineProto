---
title: messages.search
description: Search peers or messages
---
## Method: messages.search  
[Back to methods index](index.md)


Search peers or messages

### Parameters:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|important\_only|[CLICK ME Bool](../types/Bool.md) | Optional|Show only important messages|
|peer|[Username, chat ID, Update, Message or InputPeer](../types/InputPeer.md) | Optional|Where to search|
|q|[CLICK ME string](../types/string.md) | Yes|What to search|
|filter|[CLICK ME MessagesFilter](../types/MessagesFilter.md) | Yes|Message filter|
|min\_date|[CLICK ME int](../types/int.md) | Yes|Minumum date of results to fetch|
|max\_date|[CLICK ME int](../types/int.md) | Yes|Maximum date of results to fetch|
|offset|[CLICK ME int](../types/int.md) | Yes|Offset |
|max\_id|[CLICK ME int](../types/int.md) | Yes|Maximum message id to return|
|limit|[CLICK ME int](../types/int.md) | Yes|Number of results to return|


### Return type: [messages\_Messages](../types/messages_Messages.md)

### Can bots use this method: **NO**


### Errors this method can return:

| Error    | Description   |
|----------|---------------|
|CHAT_ADMIN_REQUIRED|You must be an admin in this chat to do this|
|INPUT_CONSTRUCTOR_INVALID|The provided constructor is invalid|
|INPUT_USER_DEACTIVATED|The specified user was deleted|
|PEER_ID_INVALID|The provided peer id is invalid|
|PEER_ID_NOT_SUPPORTED|The provided peer ID is not supported|
|SEARCH_QUERY_EMPTY|The search query is empty|
|USER_ID_INVALID|The provided user ID is invalid|


### MadelineProto Example:


```
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$messages_Messages = $MadelineProto->messages->search(['important_only' => Bool, 'peer' => InputPeer, 'q' => 'string', 'filter' => MessagesFilter, 'min_date' => int, 'max_date' => int, 'offset' => int, 'max_id' => int, 'limit' => int, ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/messages.search`

Parameters:

important_only - Json encoded Bool

peer - Json encoded InputPeer

q - Json encoded string

filter - Json encoded MessagesFilter

min_date - Json encoded int

max_date - Json encoded int

offset - Json encoded int

max_id - Json encoded int

limit - Json encoded int




Or, if you're into Lua:

```
messages_Messages = messages.search({important_only=Bool, peer=InputPeer, q='string', filter=MessagesFilter, min_date=int, max_date=int, offset=int, max_id=int, limit=int, })
```

