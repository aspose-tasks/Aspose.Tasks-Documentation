---
title: Utility Features
type: docs
weight: 110
url: /java/utility-features/
---

## **Calculating Critical Path**
The critical path is the tasks, or task, that ultimately determine when your project will end. Keeping track of the critical path and the resources assigned to them helps keep the project on time. Microsoft Project calculates the critical path based on tasks that have no slack, have specific date constraints (must start on, must finish on, as soon as possible or as late as possible) or have the same, or later, end date as the project. Aspose.Tasks allows you to calculate the critical path.

The [Project](https://apireference.aspose.com/tasks/java/com.aspose.tasks/project) class provides the [getCriticalPath()](https://apireference.aspose.com/tasks/java/com.aspose.tasks/Project#getCriticalPath--) method which is used to get the list of tasks that part of the critical path. 

The following piece of code calculates and displays the tasks in the critical path.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-CriticalPath-critical-path.java" >}}

## **Printing the TaskWritingException**
A project consists of a number of tasks and Aspose.Tasks API allows adding, removing and updating task information. If there's a problem when writing tasks, use TasksWritingException to catch them. 

Aspose.Tasks supports printing a message when there's an exception in writing a task. This is done with TaskWritingException, in a similar way to how TaskReadingException is used. The log message is contained in the public property TasksWritingException.getLogText(), as shown in the following code example.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-PrintTaskWritingExceptions-printing-task-writing-exceptions.java" >}}

## **Working with Filter Data from MPP files**
Aspose.Tasks allows to read Information about filters applied to an MPP file data. This topic shows retrieving Filter Definition and Filter Criteria data from a Microsoft Project MPP file.

### **Reading Filter Definition Data**
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-FilterDataFromMppFile-filter-data-definition.java" >}}
### **Reading Filter Criteria Data**
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-FilterDataFromMppFile-filter-data-criteria.java" >}}
## **Reading Group Definition Data**
A Microsoft Project data file may contain data in groups. Aspose.Tasks provides the facility to read the group definition data as shown in this topic.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ReadGroupDefinitionData-read-group-information-data.java" >}}

## **Reading Table Data from a Project File**
Aspose.Tasks API supports reading Table data from Microsoft Project data files. The Project.Tables implements the ICollection interface to provide access to the Table data of MPP file. The feature is supported for all versions of Microsoft Project data files i.e. MPP 2003, 2007, 2010 and 2013.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ReadTableDataFromFile-read-table-data-from-file.java" >}}

## **Extracting Embedded Objects from Task or Resource View**
Microsoft Project data files (MPP/XML) may contain embedded objects such as documents, excel sheets, PDF, images, etc. in Task or Resource views. Aspose.Tasks API provides the capability to extract these from a project's Task or Resource view as shown in this topic.

Embedded objects (those which were created from the file by selecting a file path) are packed into OLE Package inside MPP file. To extract the original file you can use Content and FullPath properties of an instance of the OleObject class.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ExtractingEmbeddedObjects-extracting-embedded-objects.java" >}}
