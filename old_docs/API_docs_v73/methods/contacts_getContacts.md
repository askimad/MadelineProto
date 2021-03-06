---
title: contacts.getContacts
description: Get info about a certain contact
---
## Method: contacts.getContacts  
[Back to methods index](index.md)


Get info about a certain contact

### Parameters:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|hash|[CLICK ME int](../types/int.md) | Yes|$ids is the list ids of previously fetched contacts, `$hash = $MadelineProto->gen_vector_hash($ids);`|


### Return type: [contacts\_Contacts](../types/contacts_Contacts.md)

### Can bots use this method: **NO**


### MadelineProto Example:


```
if (!file_exists('madeline.php')) {
    copy('https://phar.madelineproto.xyz/madeline.php', 'madeline.php');
}
include 'madeline.php';

$MadelineProto = new \danog\MadelineProto\API('session.madeline');
$MadelineProto->start();

$contacts_Contacts = $MadelineProto->contacts->getContacts(['hash' => int, ]);
```

### [PWRTelegram HTTP API](https://pwrtelegram.xyz) example (NOT FOR MadelineProto):



### As a user:

POST/GET to `https://api.pwrtelegram.xyz/userTOKEN/contacts.getContacts`

Parameters:

hash - Json encoded int




Or, if you're into Lua:

```
contacts_Contacts = contacts.getContacts({hash=int, })
```

