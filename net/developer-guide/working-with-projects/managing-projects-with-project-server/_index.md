---
title: Reading and Saving Projects in Project Server or Project Online
description: "Learn how to create, read or update projects in Project Server or Project Online instance using Aspose.Tasks for .NET."
type: docs
weight: 40
url: /net/managing-projects-with-project-server/
---

Aspose.Tasks for .NET supports creating/reading/updating/ of projects in Project Server on-premises instance or Project Online (cloud version of Project Server) account using PWA (Project Web Access) API.

## **Managing Projects with Project Server**
Aspose.Tasks for .NET provides the [ProjectServerManager](https://reference.aspose.com/tasks/net/aspose.tasks/projectservermanager) class to create, read and update projects in Project Server's instance or in Project Online account. The ProjectServerCredentials class shall be used to provide credentials that are used to connect to Project Online. Previously, Microsoft.SharePoint.Client.Runtime assembly was used to retrieve AuthToken but now Aspose.Tasks for .NET provides an option to specify SiteUrl, username, and password in order to create a connection to Project Online. 

*Please note that currently Aspose.Tasks for .NET cannot be used with modern authentication to Project Online. Thus legacy authentication should be enabled in your Azure portal and Office 365 Admin center.*

### **Reading Project from Project Server**
The following code example demonstrates how to read project data from Project Server.
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ExProjectServerManager-ReadingProjectOnline.cs" >}}

### **Creating a Project in Project Server**
The following code example demonstrates how to create a project in Project Server.
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ExProjectServerManager-ProjectServerManagerCreateNewProject.cs" >}}

The following code example demonstrates how to create a project with predefined save options on Microsoft Project Online.
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ExProjectServerManager-CreateProjectOnline.cs" >}}

### **Updating a Project in Project Server**
The following code example demonstrates how to update existing project in Project Server.
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ExProjectServerManager-UpdateProjectServer.cs" >}}

The following code example demonstrates how to update a project in Project Server with save options.
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ExProjectServerManager-UpdateProjectOnlineWithOptions.cs" >}}
