---
title: Attachment.Visible property (Access)
keywords: vbaac10.chm13918
f1_keywords:
- vbaac10.chm13918
api_name:
- Access.Attachment.Visible
ms.assetid: 15606b3e-dffb-f179-021a-5bf8087003a7
ms.date: 02/07/2019
ms.localizationpriority: medium
---


# Attachment.Visible property (Access)

Returns or sets whether the object is visible. Read/write **Boolean**.


## Syntax

_expression_.**Visible**

_expression_ A variable that represents an **[Attachment](Access.Attachment.md)** object.


## Remarks

To hide an object when printing, use the **DisplayWhen** property.

Use the **Visible** property to hide a control on a form or report by including the property in a macro or event procedure that runs when the **Current** event occurs. For example, you can show or hide a congratulatory message next to a salesperson's monthly sales total in a sales report, depending on the sales total.




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]