---
title: General Project Properties
type: docs
weight: 20
url: /cpp/general-project-properties/
---

## **Working with General Project Properties**
Microsoft Project saves project properties, metadata, for every project. The properties include the project's start and end dates, the current date and the status date, the type of calendar used and when a project is scheduled from. Aspose.Tasks lets you read and set project properties as described below. 
### **Reading Project Information**
The [Project]()[ ](https://apireference.aspose.com/tasks/cpp/class/aspose.tasks.project/)class has a number of properties that deal with project properties:

- [StartDate](): the project's start date, of the DateTime data type.
- [FinishDate](): the project's end date, of the DateTime data type.
- [CurrentDate](): the current date, of the DateTime data type.
- [StatusDate](): the date that the project's progress will be reported, of the DateTime data type.
- [IsScheduleFromStart](): defines whether the project is scheduled from the start or end data and takes a Boolean value.
- [Calendar](): the type of calendar used by the project, managed through the [Aspose.Tasks.Calendar]() class.

To read project properties in Microsoft Project, click **Project Information** on the **Project** menu.

![project information in MS Project 2010](working-with-project-properties_1.png)

The code example given below demonstrates how to read and output the project start and end date, whether the project is scheduled from the start or end, author, last author, revision, keywords and comments.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectProperties-ReadProjectInfo-ReadProjectInfo.cpp" >}}
### **Writing Project Information**
Aspose.Tasks for C++ can write as well as read project information. The code example given below demonstrates how to set author, last author, revision, keywords and comments.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectProperties-WriteProjectInfo-WriteProjectInfo.cpp" >}}
## **Determining Project Version**
Aspose.Tasks API provides the capability to retrieve project file information with simple API calls. The [Project]() class's [Get]() method facilitates users to retrieve Project related information using the static class [Prj](). The Prj class exposes a number of properties related to the Project. This topic shows how to retrieve version information.

The SaveVersion and LastSaved properties exposed by the Prj class are used to determine the project version and the date when the project was last saved. SaveVersion supports the Integer datatype, whereas LastSaved supports the DateTime datatype.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectProperties-DetermineProjectVersion-DetermineProjectVersion.cpp" >}}
## **Writing Project Summary Information**
Most programs save summary information with the files they save. Microsoft Project is no different. As well as the name of the author, the date the project was created and the last time it was edited and saved, it saves keywords, subject, comments and more. Aspose.Tasks lets you both read and write this type of information.

The Project's class Set method can be used to write and Get method can be used to read Project summary information using the Prj class's members. The file can be saved back after updating the summary information. To update the project summary information of an existing MPP file:

1. Create an instance of Project class
2. Set the various properties exposed by the Prj class to define summary information.
3. Save the Project using the Save method of Project class

To see the file's summary information:

1. Find the file in a file browser.
2. Right-click the file and select **Properties**.
3. Go to the **Details** tab.

The code example given below demonstrates how to write a project summary information to the MPP file.

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-WorkingWithProjects-WorkingWithProjectProperties-WriteMPPProjectSummary-WriteMPPProjectSummary.cpp" >}}
