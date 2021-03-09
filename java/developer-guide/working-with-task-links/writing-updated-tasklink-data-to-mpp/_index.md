---
title: Writing Updated TaskLink Data to MPP
type: docs
weight: 60
url: /java/writing-updated-tasklink-data-to-mpp/
---

{{% alert color="primary" %}} 

With Aspose.Tasks, it is possible to link tasks in a project and save the updated task link data back to a Microsoft Project MPP file. This means that you can open an MPP file, update task links, and save the file back out.

{{% /alert %}} 
**Updating Task Links**
The code snippet below shows how to link tasks in a project and write the link data back to the MPP file. The steps involved in this activity are:

1. Create an instance of the Project Reader.
2. Read the source MPP file.
3. Create tasks and add these to the project's root task.
4. Link the tasks using StartToFinish and FinishToStart link types.
5. Save the project using the Project Writer.

The following code demonstrates how this feature works.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-TaskLinks-UpdatedTaskLinkDataToMpp-update-task-link-data-mpp.java" >}}
