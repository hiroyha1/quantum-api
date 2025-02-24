---
uid: Microsoft.Quantum.Logical.Not
title: Not function
ms.date: 12/5/2022 12:00:00 AM
ms.topic: managed-reference
qsharp.kind: function
qsharp.namespace: Microsoft.Quantum.Logical
qsharp.name: Not
qsharp.summary: Returns the Boolean negation of a value.
---

# Not function

Namespace: [Microsoft.Quantum.Logical](xref:Microsoft.Quantum.Logical)

Package: [Microsoft.Quantum.Standard](https://nuget.org/packages/Microsoft.Quantum.Standard)


Returns the Boolean negation of a value.

```qsharp
function Not (value : Bool) : Bool
```


## Input

### value : [Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals)

The value to be negated.



## Output : [Bool](xref:microsoft.quantum.qsharp.valueliterals#bool-literals)

`true` if and only if `value` is `false`.

## Remarks

The following are equivalent:```qsharplet x = not value;let x = Not(value);```