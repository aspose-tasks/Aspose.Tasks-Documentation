---
title: Default Project Properties
type: docs
weight: 10
url: /cpp/default-project-properties/
---

## **Default Project Properties**
Microsoft Project lets users set default project properties that speed up the process of setting up a project. The default properties define when a new task starts and finishes, sets the default overtime and standard pay rates and more. Aspose.Tasks supports these features.

The [Project]() exposes a number of properties for managing a project's default properties:

- [DefaultStartTime](): a new tasks' default start time, takes a DateTime value.
- [DefaultFinishTime](): a new tasks' default finishing time, takes a DateTime value.
- [DefaultFixedCostAccrual](): an assignment's default fixed cost accrual, takes one of the values defined by the [CostAccrualType]() enumeration.
- [DefaultStandardRate](): the default standard pay rate, takes a double.
- [DefaultOvertimeRate](): the default overtime pay rate, takes a double.
- [DefaultTaskEVMethod](): the default task earned value method, takes one of the values defined by the [EarnedValueMethodType]() enumeration.
- [DefaultTaskType](): the project's default task type, takes one of the values defined by the [TaskType]() enumeration.

To see the default project information in Microsoft Project:

1. Open a project.
1. On the **Tools** menu, click **Options**.
1. Go to the **General** tab.
   Here, you can see the settings for the default standard and overtime rates.
1. Go to the **Schedule** tab.
   Here, you can see the settings for the default task type and default task start time.

**Default project information in Microsoft Project, as written by Aspose.Tasks** 

![todo:image_alt_text](/download/attachments/16286619/1924835173)
### **Reading Default Properties**
The code example given below demonstrates how to read a project's default properties and writes them to a console window.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectProperties-ReadDefaultProperties-DefaultProperties.cpp" >}}
### **Writing Default Properties**
The code example given below demonstrates how to set a project's default properties.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectProperties-WriteDefaultProperties-WriteDefaultProperties.cpp" >}}
