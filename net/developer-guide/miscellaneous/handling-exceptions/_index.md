---
title: Handling Exceptions
type: docs
weight: 20
url: /net/handling-exceptions/
---

## **Handling Exceptions**
Sometimes, Aspose customers are unable to load their projects because of unsupported features and other issues and do not want to share their projects for analysis on our [Support forums](http://www.aspose.com/community/forums/default.aspx).

The LogText property exposed by the [TasksReadingException]() class is used to deal with such cases. You can use this property to identify the problematic section of the project, for example, a problematic task, resource, resource assignment etc.

After identifying the section that's causing the problem, you can try to resolve the issue at your end or copy that data to a separate project and share with us to resolve the issue.

The following code is used to identify the cause of the exception.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-Miscellaneous-HandleExceptions-HandleExceptions.cs" >}}
