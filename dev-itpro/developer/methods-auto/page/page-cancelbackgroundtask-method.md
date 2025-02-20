---
title: "Page.CancelBackgroundTask(Integer) Method"
description: "Attempt to cancel a page background task."
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
# Page.CancelBackgroundTask(Integer) Method
> **Version**: _Available or changed with runtime version 4.0._

Attempt to cancel a page background task.


## Syntax
```AL
[Ok := ]  Page.CancelBackgroundTask(TaskId: Integer)
```
## Parameters
*Page*  
&emsp;Type: [Page](page-data-type.md)  
An instance of the [Page](page-data-type.md) data type.  

*TaskId*  
&emsp;Type: [Integer](../integer/integer-data-type.md)  
Specifies the ID of the page background task to cancel. The ID is assigned to the task when it is queued by the EnqueueBackgroundTask method.  


## Return Value
*[Optional] Ok*  
&emsp;Type: [Boolean](../boolean/boolean-data-type.md)  
**true** if the page background task was marked for cancellation; otherwise **false**.


[//]: # (IMPORTANT: END>DO_NOT_EDIT)

## Example
The following example uses the CancelBackgroundTask method to cancel an existing page background task, based on its task ID.
 
```al
var​
  WaitTaskId: Integer;​
​
trigger OnAfterGetRecord()​
var​
  TaskParameters: Dictionary of [Text, Text];​
begin​
  if (WaitTaskId > 0) then​
    Currpage.CancelBackgroundTask(WaitTaskId);​
    TaskParameters.Add('Wait', '1000');
    CurrPage.EnqueueBackgroundTask(WaitTaskId, 50100, TaskParameters, 1000, PageBackgroundTaskErrorLevel::Warning);
end;
```

CurrPage is a system-defined variable. For more information, see [System-Defined Variables](../../devenv-system-defined-variables.md). 

## See Also

[Page Background Tasks](../../devenv-page-background-tasks.md)  
[Page Data Type](page-data-type.md)  
[System-Defined Variables](../../devenv-system-defined-variables.md)  
[Getting Started with AL](../../devenv-get-started.md)  
[Developing Extensions](../../devenv-dev-overview.md)