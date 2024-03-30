---
title: SharingItem.RTFBody property (Outlook)
keywords: vbaol11.chm3537
f1_keywords:
- vbaol11.chm3537
api_name:
- Outlook.SharingItem.RTFBody
ms.assetid: c41c17c1-af15-ea13-9a31-ba1e3d0f30b2
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# SharingItem.RTFBody property (Outlook)

Returns or sets a **Byte** array that represents the body of the Microsoft Outlook item in Rich Text Format. Read/write.


## Syntax

_expression_. `RTFBody`

_expression_ A variable that represents a '[SharingItem](Outlook.SharingItem.md)' object.


## Remarks

Use the **StrConv** function in Microsoft Visual Basic for Applications (VBA), or the **System.Text.Encoding.AsciiEncoding.GetString()** method in C# or Visual Basic to convert an array of bytes to a string.


## See also


[SharingItem Object](Outlook.SharingItem.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]