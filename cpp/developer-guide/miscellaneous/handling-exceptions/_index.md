---
title: Handling Exceptions While Working with Microsoft Project Files
description: "The page contains useful scenarios of how Aspose.Tasks for C++ can be applied to handle exceptions while reading Microsoft Project (MPP/XML) files."
type: docs
weight: 20
url: /cpp/handling-exceptions/
---

## **Handling Exceptions While Working with Microsoft Project Files**
Sometimes, Aspose customers are unable to load their projects because of unsupported features and other issues and do not want to share their projects for analysis on our [Support forums](https://forum.aspose.com/c/tasks/15).

The LogText property exposed by the [TasksReadingException](https://apireference.aspose.com/tasks/cpp/_tasks_reading_exception_8h_source) class is used to deal with such cases. You can use this property to identify the problematic section of the project, for example, a problematic task, resource, resource assignment etc.

After identifying the section that's causing the problem, you can try to resolve the issue at your end or copy that data to a separate project and share with us to resolve the issue.

The following code example is used to identify the cause of the exception.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-Miscellaneous-HandleExceptions-HandleExceptions.cpp" >}}
