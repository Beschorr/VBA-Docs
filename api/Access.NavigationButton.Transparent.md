---
title: NavigationButton.Transparent property (Access)
keywords: vbaac10.chm10454
f1_keywords:
- vbaac10.chm10454
api_name:
- Access.NavigationButton.Transparent
ms.assetid: 9eab3a03-2498-f1f5-f2e1-f238859c4850
ms.date: 03/05/2019
ms.localizationpriority: medium
---


# NavigationButton.Transparent property (Access)

Use the **Transparent** property to specify whether a command button is solid or transparent. Read/write **Boolean**.


## Syntax

_expression_.**Transparent**

_expression_ A variable that represents a **[NavigationButton](Access.NavigationButton.md)** object.


## Remarks

Use the **BackStyle** property to make other controls solid or transparent.

Use this property to place a transparent command button over another control. For example, you could place several transparent buttons over a picture displayed in an image control and run various macros or Visual Basic event procedures depending on which part of the picture the user clicks.

> [!NOTE] 
> To hide and disable a button, use the **Visible** property. To disable a button without hiding it, use the **Enabled** property. To hide a button only when a form or report is printed, use the **DisplayWhen** property.


## Example

The following example makes the command button **Preview** on the **Purchase Orders** form transparent.

```vb
Forms.Item("Purchase Orders").Controls.Item("Preview"). _ 
 Transparent = True
```


[!include[Support and feedback](~/includes/feedback-boilerplate.md)]
