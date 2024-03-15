---
title: SharingItem.SenderName property (Outlook)
keywords: vbaol11.chm660
f1_keywords:
- vbaol11.chm660
api_name:
- Outlook.SharingItem.SenderName
ms.assetid: 7725b19d-23af-2084-0fca-71daaa99ba24
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# SharingItem.SenderName property (Outlook)

Returns a **String** indicating the display name of the sender for the **[SharingItem](Outlook.SharingItem.md)**. Read-only.


## Syntax

_expression_. `SenderName`

_expression_ A variable that represents a [SharingItem](Outlook.SharingItem.md) object.


## Remarks

This property corresponds to the MAPI property **PidTagSenderName**.

If you wish to retrieve the fully qualified email address of the sender, use the **[SenderEmailAddress](Outlook.SharingItem.SenderEmailAddress.md)** property.


## See also


[SharingItem Object](Outlook.SharingItem.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]