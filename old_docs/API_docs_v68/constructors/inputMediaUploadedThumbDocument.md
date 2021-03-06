---
title: inputMediaUploadedThumbDocument
description: inputMediaUploadedThumbDocument attributes, type and example
---
## Constructor: inputMediaUploadedThumbDocument  
[Back to constructors index](index.md)



### Attributes:

| Name     |    Type       | Required |
|----------|---------------|----------|
|file|[File path or InputFile](../types/InputFile.md) | Yes|
|thumb|[File path or InputFile](../types/InputFile.md) | Yes|
|mime\_type|[string](../types/string.md) | Optional|
|attributes|Array of [DocumentAttribute](../types/DocumentAttribute.md) | Yes|
|caption|[string](../types/string.md) | Yes|
|stickers|Array of [MessageMedia, Message, Update or InputDocument](../types/InputDocument.md) | Optional|



### Type: [InputMedia](../types/InputMedia.md)


### Example:

```
$inputMediaUploadedThumbDocument = ['_' => 'inputMediaUploadedThumbDocument', 'file' => InputFile, 'thumb' => InputFile, 'mime_type' => 'string', 'attributes' => [DocumentAttribute, DocumentAttribute], 'caption' => 'string', 'stickers' => [InputDocument, InputDocument]];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "inputMediaUploadedThumbDocument", "file": InputFile, "thumb": InputFile, "mime_type": "string", "attributes": [DocumentAttribute], "caption": "string", "stickers": [InputDocument]}
```


Or, if you're into Lua:  


```
inputMediaUploadedThumbDocument={_='inputMediaUploadedThumbDocument', file=InputFile, thumb=InputFile, mime_type='string', attributes={DocumentAttribute}, caption='string', stickers={InputDocument}}

```


