---
title: Update Outline Code Definitions and Values
description: "Learn how to edit outline code values and their definitions using Aspose.Tasks for .NET."
type: docs
weight: 40
url: /net/writing-updated-outline-code-definitions-and-values-to-mpp/
---

Aspose.Tasks for .NET provides the facility to add new outline code attributes to an existing Microsoft Project MPP file and save it back.

## **Updating Outline Code Definitions and Values**
The following code sample defines new outline codes and sets their various fields. The outline codes and values are then added to the project outline codes and the updated data is saved back to MPP file. The steps involved in this activity are:

1. Create an instance of Project Reader.
2. Read the source MPP file.
3. Define new OutlineValue objects and set the parameters.
4. Add the outline codes to the project's codes.
5. Save the updated project data back to the MPP file.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-Miscellaneous-UpdateOutlineCodes-UpdateOutlineCodes.cs" >}}
