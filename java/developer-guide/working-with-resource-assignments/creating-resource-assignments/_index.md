---
title: Creating Resource Assignments
description: "Learn how to create resource assignments linking tasks and resources in Microsoft Project (MPP/XML) files using Aspose.Tasks for Java."
type: docs
weight: 10
url: /java/creating-resource-assignments/
---

Resource assignments linking tasks and resources. This article explains how to create one using Aspose.Tasks for Java.

## **Creating Resource Assignments**
The [Resource](https://apireference.aspose.com/tasks/java/com.aspose.tasks/Resource) class exposes two different ways of creating a resource assignment, either using the default constructor or by passing a task and resource.

**Programming Sample: Adding ResourceAssignment to Project directly**
The following code sample adds a Resource Assignment to the project without instantiating its object.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-ResourceAssignments-CreateResourceAssignments-create-resource-assignments.java" >}}

## **Read Shared Resource Assignments**
The shared assignments are assignments of the specific resource to tasks in other projects when the current project uses a resource from a resource pool.  Using Aspose.Tasks, the shared assignments can be read from MPP and taken into account when Peak\Overallocated properties are calculated. The following code example demonstrates how to read shared resource assignments.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-ResourceAssignments-ReadSharedResourceAssignments-ReadSharedResourceAssignments.java" >}}
