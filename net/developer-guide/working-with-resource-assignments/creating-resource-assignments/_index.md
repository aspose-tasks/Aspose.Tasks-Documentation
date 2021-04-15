---
title: Creating Resource Assignments
description: "Learn how to create resource assignments linking tasks and resources in Microsoft Project (MPP/XML) files using Aspose.Tasks for .NET."
type: docs
weight: 10
url: /net/creating-resource-assignments/
---

Resource assignments are links between a task and a resource. This article explains how to create resource assignment using Aspose.Tasks for .NET.

## **Creating Resource Assignments**
The [Resource](https://apireference.aspose.com/tasks/net/aspose.tasks/resource) class exposes two different ways of creating a resource assignment, either using the default constructor or by passing a task and resource.

**Programming Sample: Default Constructor**
Create a [ResourceAssignment](https://apireference.aspose.com/tasks/net/aspose.tasks/resourceassignment) instance without requiring any parameters to be passed.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResourceAssignments-CreateResourceAssignments.cs" >}}

## **Creating Multiple Resource Assignments**
The following code example demonstrates how to set multiple resource assignments for one task and set user-defined start and end date for the resources.

{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-WorkingWithResourceAssignments-CreateMultipleResourceAssignmentsForOneTask.cs" >}}