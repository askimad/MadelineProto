---
title: getChannelMembers
description: Returns information about channel members or banned users. Can be used only if channel_full->can_get_members == true. Administrator privileges may be additionally needed for some filters
---
## Method: getChannelMembers  
[Back to methods index](index.md)


YOU CANNOT USE THIS METHOD IN MADELINEPROTO


Returns information about channel members or banned users. Can be used only if channel_full->can_get_members == true. Administrator privileges may be additionally needed for some filters

### Parameters:

| Name     |    Type       | Required | Description |
|----------|---------------|----------|-------------|
|channel\_id|[CLICK ME int](../types/int.md) | Yes|Identifier of the channel|
|filter|[CLICK ME ChannelMembersFilter](../types/ChannelMembersFilter.md) | Yes|Kind of channel users to return, defaults to channelMembersRecent|
|offset|[CLICK ME int](../types/int.md) | Yes|Number of channel users to skip|
|limit|[CLICK ME int](../types/int.md) | Yes|Maximum number of users be returned, can't be greater than 200|


### Return type: [ChatMembers](../types/ChatMembers.md)

