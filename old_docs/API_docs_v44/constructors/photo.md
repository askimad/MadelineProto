---
title: photo
description: photo attributes, type and example
---
## Constructor: photo  
[Back to constructors index](index.md)



### Attributes:

| Name     |    Type       | Required |
|----------|---------------|----------|
|id|[long](../types/long.md) | Yes|
|access\_hash|[long](../types/long.md) | Yes|
|date|[int](../types/int.md) | Yes|
|sizes|Array of [PhotoSize](../types/PhotoSize.md) | Yes|



### Type: [Photo](../types/Photo.md)


### Example:

```
$photo = ['_' => 'photo', 'id' => long, 'access_hash' => long, 'date' => int, 'sizes' => [PhotoSize, PhotoSize]];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "photo", "id": long, "access_hash": long, "date": int, "sizes": [PhotoSize]}
```


Or, if you're into Lua:  


```
photo={_='photo', id=long, access_hash=long, date=int, sizes={PhotoSize}}

```


