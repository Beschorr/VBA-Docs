---
title: Selection.BoldRun method (Word)
keywords: vbawd10.chm158663258
f1_keywords:
- vbawd10.chm158663258
api_name:
- Word.Selection.BoldRun
ms.assetid: 0998afe2-dcd9-c1e4-9614-a1af4c6bbeaf
ms.date: 05/17/2021
ms.localizationpriority: medium
---


# Selection.BoldRun method (Word)

Adds the bold character format to or removes it from the current run.

> [!IMPORTANT]
> This method has changed. Using VBA Selection commands like `Selection.BoldRun` on user selection with Comments no longer applies bold formatting on user-selected text or `Selection.TypeTxt` command or on user selection with Comments no longer inserts text.

## Syntax

_expression_. `BoldRun`

_expression_ Required. A variable that represents a **[Selection](Word.Selection.md)** object.


## Remarks

 If the run contains a mix of bold and non-bold text, this method adds the bold character format to the entire run.


## Example

This example toggles the bold formatting for the current selection.


```vb
Selection.BoldRun
```


## See also


[Selection Object](Word.Selection.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]
