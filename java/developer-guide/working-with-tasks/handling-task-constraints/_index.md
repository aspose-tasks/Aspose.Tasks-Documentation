---
title: Handling Task Constraints
type: docs
weight: 40
url: /java/handling-task-constraints/
---

{{% alert color="primary" %}} 

Task constraints are used to define a Microsoft Project project's schedule and define when tasks should be started or finished. Constraints can be flexible - start or end as soon as possible or as late as possible - or inflexible. Inflexible constraints are tied to specific dates.

{{% /alert %}} 
## **Working with Constraints**
The ConstraintDate and ConstraintType properties are exposed by the [Task](https://apireference.aspose.com/tasks/java/com.aspose.tasks/Task) class to handle constraints:

- ConstraintDate accepts and returns the Date data type.
- ConstraintType accepts and returns one of the values of the ConstraintType enumeration.
### **Setting Constraints in Microsoft Project**
To set constraints in Microsoft Project:

1. On the **View** menu, select **More Views** and then **Task Entry Form**.
2. Double click a task on the Task Entry Form.
3. Select the Advance tab.
4. Set a constraint by selecting an option from the **Constraint type** list and a date for the **Constraint date** list. 

## **Setting constraints in Microsoft Project** 

![todo:image_alt_text](handling-task-constraints_1.png)

### **Setting Constraints with Aspose.Tasks**
The constraint date is NA when the constraint type is **As Soon As Possible** or **As Late As Possible**. For date values equal to NA, Aspose.Tasks uses the value "1/1/2000” in the evaluation version, and DateTime.MinValue for the licensed product. In the below case, we take a source project file as an input and apply different types of constraints on various tasks in each case. The following code samples show the application of different Constraint types and the accompanied snapshot of the result for each case.

## **The input file** 

![todo:image_alt_text](handling-task-constraints_2.png)

The code samples below set the constraint type set to Start No Earlier Than.
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-HandleTaskConstraints-setConstraintTypeStartNoEarlierThan.java" >}}

## **Output file with Start No Earlier Than constraint** 

![todo:image_alt_text](handling-task-constraints_3.png)

The code samples below set the constraint type set to Finish No Earlier Than.
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-HandleTaskConstraints-setConstraintTypeFinishNoEarlierThan.java" >}}

## **Output file showing Finish No Earlier Than constraint** 

![todo:image_alt_text](handling-task-constraints_4.png)

The code samples below set the constraint type set to Must Start On.
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-HandleTaskConstraints-SetConstraintTypeMustStartOn.java" >}}

## **Output file showing Must Start On constraint** 

![todo:image_alt_text](handling-task-constraints_5.png)

The code samples below set the constraint type set to As Late As Possible.
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-HandleTaskConstraints-setConstraintTypeAsLateAsPossible.java" >}}

## **Output file showing As Late As Possible constraint** 

![todo:image_alt_text](handling-task-constraints_6.png)

The code sample below shows the constraint type set to Must Finish On.
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-HandleTaskConstraints-setConstraintTypeMustFinishOn.java" >}}

## **Output file showing Must Finish On constraint** 

![todo:image_alt_text](handling-task-constraints_7.png)

### **Getting Constraints**
This code sample displays any constraints found when traversing the tasks in the project to a command window.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Tasks-HandleTaskConstraints-GetConstraints.java" >}}
