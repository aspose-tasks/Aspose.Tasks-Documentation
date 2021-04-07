---
title: Writing Updated Outline Code Definitions and Values to MPP
description: "Learn how to edit outline code values and their definitions using Aspose.Tasks for C++."
type: docs
weight: 60
url: /cpp/writing-updated-outline-code-definitions-and-values-to-mpp/
---

{{% alert color="primary" %}} 

Aspose.Tasks for C++ API provides the facility to add new outline code attributes to an existing Microsoft Project MPP file and save it back.

{{% /alert %}}

## **Updating Outline Code Definitions and Values**
The following code sample defines new outline codes and sets its various fields. The outlines codes and values are then added to the project outline codes and the updated data is saved back to MPP file. The steps involved in this activity are:

1. Create an instance of Project Reader.
2. Read the source MPP file.
3. Define new OutlineValue objects and set the parameters.
4. Add the outline codes to the project's codes.
5. Save the updated project data back to the MPP file.

### **Programming Sample**

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-Miscellaneous-UpdateOutlineCodes-UpdateOutlineCodes.cpp" >}}
