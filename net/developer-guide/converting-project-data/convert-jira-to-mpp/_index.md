---
title: Export Jira tasks to MS Project MPP file
description: "Write your own converter which allows to export issues from JIRA using REST API and save them to MPP or Primavera files."
keywords: "ms project convertor, jira2mpp, microsoft project jira to mpp converter, microsoft project jira to primavera, export jira to mpp, export jira to primavera"
type: docs
weight: 60
url: /net/convert-jira-to-mpp/
---

In this article we are going to show how to export tasks from Jira using REST API to [MPP](https://docs.fileformat.com/project-management/mpp/) file format using Aspose.Tasks for .NET.

## **Export Jira tasks to MPP**

Here is the simplified code which demonstrates the key ideas which allows your to build your own solution to export Jira tasks to MPP or any export format supported by Aspose.Tasks for .NET.

In order to export tasks from Jira to MPP format the following steps should be performed:

1. Make a request to Jira API to select the tasks to export.
2. Create an instance of Project class.
2. Traverse the resulting JSON and create a Task object for each "issue" entity in the resulting JSON.
3. Implement logic for setting Task.Start, Finish and Duration fields.
4. Save the instance of Project class to a file in the required format (MPP in this example).

{{< gist "sva1000" "afe8b1a71f5c781b4a97826e449d8124" "JiraToMpp.cs" >}}