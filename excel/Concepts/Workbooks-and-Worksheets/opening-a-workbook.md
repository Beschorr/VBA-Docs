---
title: Opening a Workbook
keywords: vbaxl10.chm5203418
f1_keywords:
- vbaxl10.chm5203418
ms.assetid: d7445059-fcb3-edf3-752e-3a1014022f81
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# Opening a Workbook

When you open a workbook using the **[Open](../../../api/Excel.Workbooks.Open.md)** method, it becomes a member of the **[Workbooks](../../../api/Excel.Workbooks.md)** collection. The following procedure opens a workbook named MyBook.xls located in the folder named MyFolder on drive C.


```vb
Sub OpenUp() 
 Workbooks.Open("C:\MyFolder\MyBook.xls") 
End Sub
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]
