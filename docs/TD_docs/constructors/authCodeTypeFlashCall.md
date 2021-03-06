---
title: authCodeTypeFlashCall
description: Code is delivered by the immediately cancelled call to the specified phone number. Number from which the call was done is the code
---
## Constructor: authCodeTypeFlashCall  
[Back to constructors index](index.md)



Code is delivered by the immediately cancelled call to the specified phone number. Number from which the call was done is the code

### Attributes:

| Name     |    Type       | Required | Description |
|----------|:-------------:|:--------:|------------:|
|pattern|[string](../types/string.md) | Yes|Pattern of the phone number from which the call will be done|



### Type: [AuthCodeType](../types/AuthCodeType.md)


### Example:

```
$authCodeTypeFlashCall = ['_' => 'authCodeTypeFlashCall', 'pattern' => 'string'];
```  

[PWRTelegram](https://pwrtelegram.xyz) json-encoded version:

```
{"_": "authCodeTypeFlashCall", "pattern": "string"}
```


Or, if you're into Lua:  


```
authCodeTypeFlashCall={_='authCodeTypeFlashCall', pattern='string'}

```


