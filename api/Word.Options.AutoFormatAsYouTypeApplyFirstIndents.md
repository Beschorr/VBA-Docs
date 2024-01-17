---
title: Options.AutoFormatAsYouTypeApplyFirstIndents property (Word)
keywords: vbawd10.chm162988329
f1_keywords:
- vbawd10.chm162988329
api_name:
- Word.Options.AutoFormatAsYouTypeApplyFirstIndents
ms.assetid: d6995d25-194f-8792-38c6-57db562c332b
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# Options.AutoFormatAsYouTypeApplyFirstIndents property (Word)

 **True** for Microsoft Word to automatically replace a space entered at the beginning of a paragraph with a first-line indent. Read/write.


## Syntax

_expression_. `AutoFormatAsYouTypeApplyFirstIndents`

_expression_ Required. A variable that represents an **[Options](Word.Options.md)** object.


## Example

This example sets Microsoft Word to automatically replace a space entered at the beginning of a paragraph with a first-line indent as you type.


```vb
Sub ApplyFirstIndents() 
 Options.AutoFormatAsYouTypeApplyFirstIndents = True 
End Sub
```


## See also


[Options Object](Word.Options.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]