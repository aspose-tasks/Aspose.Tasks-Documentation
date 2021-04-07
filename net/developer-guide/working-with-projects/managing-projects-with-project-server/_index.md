---
title: Managing Projects with Project Server
description: "Learn how to read projects from PProject Server using Aspose.Tasks for .NET."
type: docs
weight: 30
url: /net/managing-projects-with-project-server/
---

Aspose.Tasks for .NET is supporting a reading projects from Project Server database.

## **Managing Projects with Project Server**
Aspose.Tasks for .NET provides the ProjectServerManager class to create, read and update projects in Project Server. The [ProjectServerManager ](https://apireference.aspose.com/tasks/net/aspose.tasks/projectservermanager)class provides the methods to retrieve projects from the specified Project Online account. The ProjectServerCredentials class shall be used to provide credentials that are used to connect to Project Online. Previously, Microsoft.SharePoint.Client.Runtime assembly was used to retrieve AuthToken but now Aspose.Tasks for .NET provides an option to specify SiteUrl, username, and password in order to create a connection to Project Online.  

### **Reading Project from Project Server**
The following code example demonstrates how to read project data from Project Server.
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ExProjectServerManager-ReadingProjectOnline.cs" >}}

### **Creating a Project in Project Server**
The following code example demonstrates how to create a project in Project Server.
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ExProjectServerManager-ProjectServerManagerCreateNewProject.cs" >}}

The following code example demonstrates how to create a project with predefined save options on Microsoft Project Online.
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ExProjectServerManager-CreateProjectOnline.cs" >}}

### **Updating a Project in Project Server**
The following code example demonstrates how to update a project in Project Server.
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ExProjectServerManager-UpdateProjectServer.cs" >}}

The following code example demonstrates how to update a project in Project Server with save options.
{{< gist "aspose-com-gists" "10d4de13018b7279cf03bab28ed78aeb" "Examples-CSharp-ExProjectServerManager-UpdateProjectOnlineWithOptions.cs" >}}
