---
title: Handling Exceptions using Aspose.Tasks
description: "The page contains useful scenarios of how Aspose.Tasks for Java can be applied to handle exceptions while reading Microsoft Project (MPP/XML) files."
type: docs
weight: 10
url: /java/handling-exceptions/
---

## **Handling Exceptions While Working with Microsoft Project Files**
Sometimes, Aspose customers are unable to load their projects because of unsupported features and other issues and do not want to share their projects for analysis on our [Support forums](https://forum.aspose.com/c/tasks/15).

The LogText property exposed by the [TasksReadingException](https://apireference.aspose.com/tasks/java/com.aspose.tasks/tasksreadingexception) class is used to deal with such cases. You can use this property to identify the problematic section of the project, for example, a problematic task, resource, resource assignment etc.

After identifying the section that's causing the problem, you can try to resolve the issue at your end or copy that data to a separate project and share with us to resolve the issue.

The following code is used to identify the cause of the exception.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Miscellaneous-HandleExceptions-handling-exceptions.java" >}}
