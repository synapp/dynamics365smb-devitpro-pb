---
title: "XmlElement.Create(String, String) Method"
description: "Creates an XmlElement node."
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
# XmlElement.Create(String, String) Method
> **Version**: _Available or changed with runtime version 1.0._

Creates an XmlElement node.


## Syntax
```AL
XmlElement :=   XmlElement.Create(LocalName: String, NamespaceUri: String)
```
## Parameters
*LocalName*  
&emsp;Type: [String](/dynamics365/business-central/dev-itpro/developer/methods-auto/text/text-data-type)  
The local name of the element to create.
        
*NamespaceUri*  
&emsp;Type: [String](/dynamics365/business-central/dev-itpro/developer/methods-auto/text/text-data-type)  
The namespace URI of the element to create.  


## Return Value
*XmlElement*  
&emsp;Type: [XmlElement](xmlelement-data-type.md)  
The created XmlElement node.


[//]: # (IMPORTANT: END>DO_NOT_EDIT)
## See Also
[XmlElement Data Type](xmlelement-data-type.md)  
[Getting Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)