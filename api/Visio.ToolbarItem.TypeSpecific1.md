---
title: ToolbarItem.TypeSpecific1 property (Visio)
keywords: vis_sdr.chm13514600
f1_keywords:
- vis_sdr.chm13514600
api_name:
- Visio.ToolbarItem.TypeSpecific1
ms.assetid: e282f50e-ec10-1c6d-5ccd-33887882735f
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# ToolbarItem.TypeSpecific1 property (Visio)

Gets or sets the type of a toolbar item. Read/write.


## Syntax

_expression_. `TypeSpecific1`

_expression_ A variable that represents a **[ToolbarItem](Visio.ToolbarItem.md)** object.


## Return value

Integer


## Remarks

The value of an object's **TypeSpecific1** property depends on the value of its **CntrlType** property.



|**CntrlType value **|**TypeSpecific1 value **|
|:-----|:-----|
| **visCtrlTypeBUTTON**|Any constant prefixed with **visIconIX** that is declared by the Visio type library.|
| **visCtrlTypeCOMBOBOX**|Zero (0).|
| **visCtrlTypeEDITBOX**|Zero (0).|
| **visCtrlTypeLABEL**|The **TypeSpecific1** property is not used.|

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]