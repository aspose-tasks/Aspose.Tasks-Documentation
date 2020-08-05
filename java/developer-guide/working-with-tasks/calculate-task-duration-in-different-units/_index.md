---
title: Calculate Task Duration in Different Units
type: docs
weight: 200
url: /java/calculate-task-duration-in-different-units/
---

{{% alert color="primary" %}} 

It can be useful to calculate the duration of a task in different units such as minutes, hours, etc.

{{% /alert %}} 
## **Calculating Durations**
The [Task](http://www.aspose.com/api/java/tasks/com.aspose.tasks/classes/Task) class offers provides the getDuration() method for calculating task duration in different units. This method takes TimeUnitType as the input argument and returns the duration as a double value.

**Programming Sample**

The following piece of code shows how to use this method to retrieve a task's duration in different units: minute, day, hour, week and month.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-TaskDurationInDifferentUnits-calculate-task-duration-in-different-units.java" >}}
