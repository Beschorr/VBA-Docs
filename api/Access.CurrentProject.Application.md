---
title: CurrentProject.Application property (Access)
keywords: vbaac10.chm12722
f1_keywords:
- vbaac10.chm12722
api_name:
- Access.CurrentProject.Application
ms.assetid: 565628df-7dbc-be17-9c8a-80de222a1583
ms.date: 02/27/2019
ms.localizationpriority: medium
---


# CurrentProject.Application property (Access)

Use the **Application** property to access the active Microsoft Access **[Application](Access.Application.md)** object and its related properties. Read-only **Application** object.


## Syntax

_expression_.**Application**

_expression_ A variable that represents a **[CurrentProject](Access.CurrentProject.md)** object.


## Remarks

The **Application** property is set by Microsoft Access and is read-only in all views.

Each Microsoft Access object has an **Application** property that returns the current **Application** object. Use this property to access any of the object's properties. For example, you could refer to the menu bar for the **Application** object from the current form by using the following syntax.

```vb
Me.Application.MenuBar 

```




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]