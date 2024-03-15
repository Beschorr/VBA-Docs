---
title: Table.MoveToStart method (Outlook)
keywords: vbaol11.chm2233
f1_keywords:
- vbaol11.chm2233
api_name:
- Outlook.Table.MoveToStart
ms.assetid: af499471-dd21-9374-7399-3ce977368015
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# Table.MoveToStart method (Outlook)

Moves the current row of the **[Table](Outlook.Table.md)** to just before the first row of the **Table**.


## Syntax

_expression_. `MoveToStart`

_expression_ A variable that represents a [Table](Outlook.Table.md) object.


## Remarks

 **MoveToStart** is equivalent to resetting the **Table**. If you call **[GetNextRow](Outlook.Table.GetNextRow.md)** after you call **MoveToStart**, you'll return a row representing the first row in the **Table**.


## See also


[Table Object](Outlook.Table.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]