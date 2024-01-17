---
title: Control.Report property (Access)
keywords: vbaac10.chm10140
f1_keywords:
- vbaac10.chm10140
api_name:
- Access.Control.Report
ms.assetid: 1c1f4703-bda7-de97-eb13-830238a5170a
ms.date: 03/06/2019
ms.localizationpriority: medium
---


# Control.Report property (Access)

Use the **Report** property to refer to a report or to refer to the report associated with a subreport control. Read-only **Report**.


## Syntax

_expression_.**Report**

_expression_ A variable that represents a **[Control](Access.Control.md)** object.


## Remarks

This property is typically used to refer to the report contained in a subreport control.

When you use the **[Reports](Access.Reports.md)** collection, you must specify the name of the report.


## Example

The following example uses the **Report** property to refer to a control on a subreport.

```vb
Dim curTotalSales As Currency 
 
curTotalSales = Reports!Sales!Employees.Report!TotalSales
```




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]