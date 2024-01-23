---
title: InvisibleApp.LanguageHelp property (Visio)
keywords: vis_sdr.chm17551700
f1_keywords:
- vis_sdr.chm17551700
api_name:
- Visio.InvisibleApp.LanguageHelp
ms.assetid: 58dc3f31-84c3-6b94-4460-c648dfff22d6
ms.date: 06/26/2019
ms.localizationpriority: medium
---


# InvisibleApp.LanguageHelp property (Visio)

Represents the language ID of the Help in the version of the Microsoft Visio instance represented by the parent object. Read-only.


## Syntax

_expression_.**LanguageHelp**

_expression_ A variable that represents an **[InvisibleApp](Visio.InvisibleApp.md)** object.


## Return value

Long


## Remarks

The **LanguageHelp** property returns the language ID of the Help recorded in the object's VERSIONINFO resource. The IDs returned are the standard IDs used by Windows to encode different language versions. For example, the **LanguageHelp** property returns &H0409 for the U.S. English version of Visio. 

For more information, see [Version information](/windows/desktop/menurc/version-information).

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]