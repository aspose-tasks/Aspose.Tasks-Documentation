---
title: Task's General Properties
description: "Learn how to work with Microsoft Project (MPP/XML) general properties using Aspose.Tasks for C++."
type: docs
weight: 20
url: /cpp/general-properties/
---

{{% alert color="primary" %}} 

Tasks can be identified by a number of general properties, such as name, ID, start and finish date. Aspose.Tasks can be used to get and set task properties when working with projects.

{{% /alert %}}

## **Overview**
The static class Tsk contains all the properties related to a Task and can get or set using the Get and Set methods exposed by Task class. Some of the commonly used properties are as follow:

- Name, used to set and get a task's name (string).
- Id, used to set and get a task's ID (integer).
- Uid, used to set and get a task's unique ID (integer).
- Start, used to set and get a task's start date (DateTime).
- Finish, used to set and get a task's end date (DateTime).

To view a task's general properties in Microsoft Project:

1. Open a project.
2. On the **View** menu, select **More Views** and then **Task Entry** to open the task entry form.
3. From the **Insert** menu, select **Column** and add the **ID** and **Unique ID**.

### **Setting General Properties**
The code example given below demonstrates how to set general properties.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-WriteTaskProperties-WriteTaskProperties.cpp" >}}

### **Getting General Properties**
Get a task's properties by traversing the children of the project's RootTask property.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithTasks-ReadTaskProperties-ReadTaskProperties.cpp" >}}
