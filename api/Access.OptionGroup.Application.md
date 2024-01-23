---
title: OptionGroup.Application property (Access)
keywords: vbaac10.chm10809
f1_keywords:
- vbaac10.chm10809
api_name:
- Access.OptionGroup.Application
ms.assetid: 21d0325e-4552-699e-4972-1fc5ee157b21
ms.date: 06/08/2019
ms.localizationpriority: medium
---


# OptionGroup.Application property (Access)

Use the **Application** property to access the active Microsoft Access **[Application](Access.Application.md)** object and its related properties. Read-only **Application** object.


## Syntax

_expression_.**Application**

_expression_ A variable that represents an **[OptionGroup](Access.OptionGroup.md)** object.


## Remarks

The **Application** property is set by Microsoft Access and is read-only in all views.

Each Microsoft Access object has an **Application** property that returns the current **Application** object. Use this property to access any of the object's properties. For example, you could refer to the menu bar for the **Application** object from the current form by using the following syntax.

```vb
Me.Application.MenuBar 

```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]