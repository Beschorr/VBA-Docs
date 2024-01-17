---
title: ListBox.Visible property (Access)
keywords: vbaac10.chm11233
f1_keywords:
- vbaac10.chm11233
api_name:
- Access.ListBox.Visible
ms.assetid: 76361c20-b6b4-6d75-e732-2e63b2c8485e
ms.date: 02/27/2019
ms.localizationpriority: medium
---


# ListBox.Visible property (Access)

Returns or sets whether the object is visible. Read/write **Boolean**.


## Syntax

_expression_.**Visible**

_expression_ A variable that represents a **[ListBox](Access.ListBox.md)** object.


## Remarks

To hide an object when printing, use the **DisplayWhen** property.

Use the **Visible** property to hide a control on a form or report by including the property in a macro or event procedure that runs when the **Current** event occurs. For example, you can show or hide a congratulatory message next to a salesperson's monthly sales total in a sales report, depending on the sales total.




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]