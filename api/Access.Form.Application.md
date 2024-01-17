---
title: Form.Application property (Access)
keywords: vbaac10.chm13489
f1_keywords:
- vbaac10.chm13489
api_name:
- Access.Form.Application
ms.assetid: decaf70d-da61-6d74-9f60-8008a3c2e00f
ms.date: 03/09/2019
ms.localizationpriority: medium
---


# Form.Application property (Access)

Use the **Application** property to access the active Microsoft Access **[Application](Access.Application.md)** object and its related properties. Read-only **Application** object.


## Syntax

_expression_.**Application**

_expression_ A variable that represents a **[Form](Access.Form.md)** object.


## Remarks

The **Application** property is set by Microsoft Access and is read-only in all views.

Each Microsoft Access object has an **Application** property that returns the current **Application** object. Use this property to access any of the object's properties. For example, you could refer to the menu bar for the **Application** object from the current form by using the following syntax.

```vb
Me.Application.MenuBar 

```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]