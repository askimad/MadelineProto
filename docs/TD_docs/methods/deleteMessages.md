---
title: deleteMessages
description: Deletes messages
---
## Method: deleteMessages  
[Back to methods index](index.md)


YOU CANNOT USE THIS METHOD IN MADELINEPROTO


Deletes messages

### Parameters:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|chat\_id|[CLICK ME int53](../types/int53.md) | Yes|Chat identifier|
|message\_ids|Array of [CLICK ME int53](../types/int53.md) | Yes|Identifiers of messages to delete|
|revoke|[CLICK ME Bool](../types/Bool.md) | Yes|Pass true to try to delete sent messages for all chat members (may fail if messages are too old). Is always true for Channels and SecretChats|


### Return type: [Ok](../types/Ok.md)

