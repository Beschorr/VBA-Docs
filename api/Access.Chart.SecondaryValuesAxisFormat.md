---
title: Chart.SecondaryValuesAxisFormat property (Access)
keywords: vbaac10.chm6165
f1_keywords:
- vbaac10.chm6165
api_name:
- Access.Chart.SecondaryValuesAxisFormat
ms.date: 11/28/2018
ms.localizationpriority: medium
---


# Chart.SecondaryValuesAxisFormat property (Access)

Returns or sets the format of the values on the secondary values axis. Read/write **String**.

Use a [predefined or custom format](Access.format.propertynumber.and.currency.md).


## Syntax

_expression_.**SecondaryValuesAxisFormat**

_expression_ A variable that represents a **[Chart](Access.Chart.md)** object.


## Example

```vb
With myChart
 .PrimaryValuesAxisFormat = "#,###.#0"
 .SecondaryValuesAxisFormat = "Currency"
End With
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]