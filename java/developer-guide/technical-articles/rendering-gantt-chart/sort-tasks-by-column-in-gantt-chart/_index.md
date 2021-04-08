---
title: Sort Tasks by Column in Gantt Chart
description: "Learn how to sort tasks by any column defined in Gantt chart view using Aspose.Tasks for Java."
type: docs
weight: 10
url: /java/sort-tasks-by-column-in-gantt-chart/
---

{{% alert color="primary" %}} 

Aspose.Tasks for Java provides the ability to sort tasks by any column in the Gantt chart view. This is accomplished with the help of the comparer method saveOptions.setTasksComparer before rendering in Gantt chart. The default comparer sorts tasks by task ID if no other option is specified.

{{% /alert %}}

## **Sort Tasks**
{{< highlight java >}}
Project project = new Project();
project.addTask("B Task 1");
project.addTask("A Task 2");
SaveOptions options = new PdfSaveOptions();
BarStyle barStyle = new BarStyle();
barStyle.setBarTextConverter(new BarStyle.TaskToBarTextConverter() {
    //@Override
    public String invoke(Task task) { return task.getName(); }
} );
barStyle.setBarColor(java.awt.Color.BLUE);
List<BarStyle> styles = new LinkedList<BarStyle>();
styles.add(barStyle);
options.setBarStyles(styles);
options.setTasksComparer(new TaskNameComparator());
project.save("output.pdf", options);

// ...

private static class TaskNameComparator implements Comparator<Task>
{
    //@Override
    public int compare(Task o1, Task o2) {
        return o1.getName().compareTo(o2.getName());
    }
}
{{< /highlight >}}
