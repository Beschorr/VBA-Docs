---
title: Project.Calendar property (Project)
ms.service: project-server
api_name:
- Project.Project.Calendar
ms.assetid: 0496a31e-7469-57e0-7675-ac9c6677f992
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# Project.Calendar property (Project)

Gets a **[Calendar](Project.Calendar.md)** object representing a calendar for the project. Read-only **Calendar**.


## Syntax

_expression_. `Calendar`

_expression_ A variable that represents a **[Project](project.project.md)** object.


## Example

The following example resets the calendar for the active project.


```vb
Sub ResetActiveProjectCalendar() 
 ActiveProject.Calendar.Reset 
End Sub
```

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]