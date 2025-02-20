---
title: "RecordRef.CurrentCompany() Method"
description: "Gets the current company of a database table referred to by a RecordRef."
ms.author: solsen
ms.custom: na
ms.date: 07/07/2021
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: reference
author: SusanneWindfeldPedersen
---
[//]: # (START>DO_NOT_EDIT)
[//]: # (IMPORTANT:Do not edit any of the content between here and the END>DO_NOT_EDIT.)
[//]: # (Any modifications should be made in the .xml files in the ModernDev repo.)
# RecordRef.CurrentCompany() Method
> **Version**: _Available or changed with runtime version 1.0._

Gets the current company of a database table referred to by a RecordRef.


## Syntax
```AL
Company :=   RecordRef.CurrentCompany()
```
> [!NOTE]
> This method can be invoked using property access syntax.

## Parameters
*RecordRef*  
&emsp;Type: [RecordRef](recordref-data-type.md)  
An instance of the [RecordRef](recordref-data-type.md) data type.  

## Return Value
*Company*  
&emsp;Type: [String](/dynamics365/business-central/dev-itpro/developer/methods-auto/text/text-data-type)  
The name of the current company.


[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also
[RecordRef Data Type](recordref-data-type.md)  
[Getting Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)