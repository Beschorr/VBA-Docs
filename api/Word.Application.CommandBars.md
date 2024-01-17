---
title: Application.CommandBars property (Word)
description: Learn how to return a CommandBars collection that represents the menu bar (Word)
keywords: vbawd10.chm158335033
f1_keywords:
- vbawd10.chm158335033
api_name:
- Word.Application.CommandBars
ms.assetid: 1082697d-edc8-c619-40d1-466d2ebf3817
ms.date: 07/20/2021
ms.localizationpriority: medium
---


# Application.CommandBars property (Word)

Returns a **CommandBars** collection that represents the menu bar and all the toolbars in Microsoft Word.

>[!Important]
>This property has changed. **CommandBars**("Comments") cannot be used to customize the context menu for comments.

## Syntax

_expression_.**CommandBars**

_expression_ A variable that represents an **[Application](Word.Application.md)** object. 


## Remarks

Use the **[CustomizationContext](Word.Application.CustomizationContext.md)** property to set the template or document context prior to accessing the **CommandBars** collection.

For information about returning a single member of a collection, see [Returning an object from a collection](../word/Concepts/Miscellaneous/returning-an-object-from-a-collection-word.md).


## Example

This example enlarges all command bar buttons and enables ToolTips.

```vb
With CommandBars 
 .LargeButtons = True 
 .DisplayTooltips = True 
End With
```

This example displays the **Drawing** toolbar at the bottom of the application window.

```vb
With CommandBars("Drawing") 
 .Visible = True 
 .Position = msoBarBottom 
End With
```

This example adds the Versions command button to the **Standard** toolbar.

```vb
CustomizationContext = NormalTemplate 
CommandBars("Standard").Controls.Add Type:=msoControlButton, _ 
 ID:=2522, Before:=4
```

## See also

[Application Object](Word.Application.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]
