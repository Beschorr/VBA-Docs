---
title: Application.WindowDeactivate event (Project)
ms.service: project-server
api_name:
- Project.Application.WindowDeactivate
ms.assetid: 141940d7-f117-d3a8-2aa5-83679a5fbfd4
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# Application.WindowDeactivate event (Project)

Occurs when any window within Project is deactivated. The **WindowDeactivate** event does not occur when the application window is deactivated.


## Syntax

_expression_.**WindowDeactivate** (_deactivatedWindow_)

_expression_ A variable that represents an **[Application](Project.Application.md)** object.


## Parameters

|Name|Required/Optional|Data type|Description|
|:-----|:-----|:-----|:-----|
| _deactivatedWindow_|Required|**Window**| The deactivated window.|

## Return value

**Nothing**


## Remarks

Project events don't occur when the project is embedded in another document or application.

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]