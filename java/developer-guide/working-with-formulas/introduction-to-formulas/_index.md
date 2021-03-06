---
title: Introduction to Formulas
description: "The page contains an introduction in project formula grammar that used by Aspose.Tasks for Java library for calculations."
type: docs
weight: 10
url: /java/introduction-to-formulas/
---

Aspose.Tasks for Java API supports reading/writing formulas to MPP project files. The Formula property of the ExtendedAttributeDefinition provides the interface for reading the formula value. This section describes how to read formulas from local as well as Enterprise Extended Attributes from the MPP file.

When assigning an invalid formula string to the instance of ExtendedAttributeDefinition class, FormatException is thrown.

**Formula Grammar**
Microsoft Project uses the following grammar for formula.

{{< highlight text >}}
Formula -> Formula Binary_Op Primary | Primary
Primary -> (Formula) | Unary_Op Primary | Function | [ValidFieldName] | ValidDoubleValue | "StringLiteral"
Function -> ValidFunctionName(Args)
Args -> Args Delimiter Formula | Formula | |
Delimiter -> , | ; Note that Delimiter is culture-specific in xml format ( , or ; ) and persistent in mpp ( , )
Binary_Op -> + | - | * | / | & | MOD | ^ | = | <> | < | >| AND | OR
Unary_Op -> NOT | + | -
{{< /highlight >}}
