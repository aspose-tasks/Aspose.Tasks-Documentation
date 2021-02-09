---
title: Defining Link Type
type: docs
weight: 20
url: /net/defining-link-type/
---

{{% alert color="primary" %}} 

The [LinkType](https://apireference.aspose.com/tasks/net/aspose.tasks/tasklink/properties/linktype) property exposed by the [TaskLink](https://apireference.aspose.com/tasks/net/aspose.tasks/tasklink) class is used to retrieve or define the type of link between two tasks. It reads and writes one of the values defined by the [TaskLinkType](https://apireference.aspose.com/tasks/net/aspose.tasks/tasklinktype) enumeration type.

{{% /alert %}} 
## **Defining Link Type**
To define link type in Microsoft Project:
On the **View** menu, select **More Views** and then **Task Entry Form**.

1. Double-click the desired task.
1. Select the **Predecessor** tab.


**Defining link type in Microsoft Project** 

![todo:image_alt_text](defining-link-type_1.png)
### **Setting Link Type with Aspose.Tasks**
The code samples below set a link type as “Start-to-Start”, the default link type is “Finish-to-Start”.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTaskLinks-SetTaskLinkType-SetTaskLinkType.cs" >}}
### **Getting Link Type with Aspose.Tasks**
The code samples below display link types by traversing the task links in the project and printing the result to a console window.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithTaskLinks-GetTaskLinkType-GetTaskLinkType.cs" >}}
