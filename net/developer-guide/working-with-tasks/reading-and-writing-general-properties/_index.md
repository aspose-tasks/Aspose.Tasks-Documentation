---
title: Reading and Writing General Properties
description: "Learn how to work with Microsoft Project (MPP/XML) general properties using Aspose.Tasks for .NET."
type: docs
weight: 20
url: /net/reading-and-writing-general-properties/
---

Tasks can be identified by a number of general properties, such as name, ID, start and finish date. Aspose.Tasks can be used to get and set task properties when working with projects.

## **General Properties**
The static class [Tsk](https://apireference.aspose.com/tasks/net/aspose.tasks/tsk) contains all the properties related to a [Task](https://apireference.aspose.com/email/net/aspose.email.calendar/task) and can be get or set using the Get and Set methods exposed by Task. Some of the commonly used properties are as follow:

- Name, used to set and get a task's name (string).
- Id, used to set and get a task's ID (integer).
- Uid, used to set and get a task's unique ID (integer).
- Start, used to set and get a task's start date (DateTime).
- Finish, used to set and get a task's end date (DateTime).

To view a task's general properties in Microsoft Project:

1. Open a project.
2. On the **View** menu, select **More Views** and then **Task Entry** to open the task entry form.
3. From the **Insert** menu, select **Column** and add the **ID** and **Unique ID**.

### **Setting General Properties**
The below code sample shows you, how to set general properties.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-WriteTaskProperties-WriteTaskProperties.cs" >}}

### **Getting General Properties**
Get a task's properties by traversing the children of the project's RootTask property.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTasks-ReadTaskProperties-ReadTaskProperties.cs" >}}
