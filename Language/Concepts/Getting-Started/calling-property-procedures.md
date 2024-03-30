---
title: Calling property procedures (VBA)
keywords: vbcn6.chm1101365
f1_keywords:
- vbcn6.chm1101365
ms.assetid: 37dfc0de-5db0-85bd-0c15-6d876b6abff9
ms.date: 12/21/2018
ms.localizationpriority: medium
---


# Calling property procedures

The following table lists the syntax for calling property procedures:

|Property procedure|Syntax|
|:-----|:-----|
|**[Property Get](../../reference/user-interface-help/property-get-statement.md)**|[**Set** \|[**Let** ]] _varname_ = [ _object_.] _propname_ [( [_arguments_] )]|
|**[Property Let](../../reference/user-interface-help/property-let-statement.md)**|[**Let** ] [ _object_.] _propname_ [( [_arguments_] )] = _argument_|
|**[Property Set](../../reference/user-interface-help/property-set-statement.md)**| **Set** [ _object_.] _propname_ [( [_arguments_] )] = _objectArg_|

When you call a **Property Let** or **Property Set** procedure, one [argument](../../Glossary/vbe-glossary.md#argument) always appears on the right side of the equal sign (**=**).

When you declare a **Property Let** or **Property Set** procedure with multiple arguments, Visual Basic passes the argument on the right side of the call to the last argument in the **Property Let** or **Property Set** declaration.

For example, the following diagram shows how arguments in the property procedure call relate to arguments in the **Property Let** declaration:

![Property Let](../../../images/abhlp002_ZA01201812.gif)

The following code example demonstrates the relationship between property procedure arguments and parameters.

```vb:DemoType.cls
'DemoType class declaration
Private pW
Private pX
Private pY
Private pZ

Property Get DemoProperty(w, x, y)
    'Calling format is: `z = DemoProperty(w, x, y)`
    ' or `Set z = DemoProperty(w, x, y)`
    w = pW
    x = pX
    y = pY
    If IsObject(pZ) Then
        Set DemoProperty = pZ
    Else
        DemoProperty = pZ
    End If
End Property
Property Let DemoProperty(w, x, y, z)
    'Calling format is `DemoProperty(w, x, y) = z`
    pW = w
    pX = x
    pY = y
    pZ = z
End Property
Property Set DemoProperty(w, x, y, z As Object)
    'Calling format is `Set DemoProperty(w, x, y) = z`
    pW = w
    pX = x
    pY = y
    Set pZ = z
End Property
```

```vb:DemoCodeModule.bas
Sub DemoSub()
    Dim myDemo As Object
    Dim a, b, c, d
    Dim w, x, y, z

    Set myDemo = New DemoType

    a = "Hello"
    b = ", "
    c = "world"
    d = "!"

    Debug.Print Join(Array(a, b, c, d), "") ' Hello, world!

    'Call Property Let DemoProperty(a, b, c, d)
    Let myDemo.DemoProperty(a, b, c) = d
    'Call Property Get
    d = myDemo.DemoProperty(a, b, c)

    Debug.Print Join(Array(a, b, c, d), "") ' Hello, world!
End Sub
```

In practice, the only use for property procedures with multiple arguments is to create [arrays](../../Glossary/vbe-glossary.md#array) of [properties](../../Glossary/vbe-glossary.md#property).

## See also

- [Visual Basic conceptual topics](../../reference/user-interface-help/visual-basic-conceptual-topics.md)
  - [Writing a property procedure](./writing-a-property-procedure.md)
  - [Executing code when setting properties](./executing-code-when-setting-properties.md)
- [Visual Basic Statements](../../reference/statements.md)
  - [Property Let](../../reference/user-interface-help/property-let-statement.md)
  - [Property Set](../../reference/user-interface-help/property-set-statement.md)
  - [Property Get](../../reference/user-interface-help/property-get-statement.md)
- [Visual Basic user interface Error messages](../../Reference/error-messages.md)
  - [Error: "Definitions of property procedures for the same property are inconsistent"](../../Reference/User-Interface-Help/definitions-of-property-procedures-for-the-same-property-are-inconsistent.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]
