---
title: TabControl.IsVisible property (Access)
keywords: vbaac10.chm12102
f1_keywords:
- vbaac10.chm12102
api_name:
- Access.TabControl.IsVisible
ms.assetid: ddc5e22d-f426-a685-ab94-a1ae7c00e53a
ms.date: 02/22/2019
ms.localizationpriority: medium
---


# TabControl.IsVisible property (Access)

Use the **IsVisible** property to determine whether a control on a report is visible. Read/write **Boolean**.


## Syntax

_expression_.**IsVisible**

_expression_ A variable that represents a **[TabControl](Access.TabControl.md)** object.


## Remarks

You can set the **IsVisible** property only in the **Print** event of a report section that contains the control.

Use the **IsVisible** property together with the **HideDuplicates** property to determine when a control on a report is visible and show or hide other controls as a result. For example, you could hide a line control when a text box control is hidden because it contains duplicate values.


## Example

The following example uses the **IsVisible** property of a text box to control the display of a line control on a report. 

Paste the following code into the Declarations section of the report module, and then view the report to see the line formatting controlled by the **IsVisible** property.

```vb
Private Sub Detail_Print(Cancel As Integer, PrintCount As Integer) 
 If Me!CategoryID.IsVisible Then 
 Me!Line0.Visible = True 
 Else 
 Me!Line0.Visible = False 
 End If 
End Sub
```


[!include[Support and feedback](~/includes/feedback-boilerplate.md)]