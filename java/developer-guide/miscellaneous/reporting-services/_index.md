---
title: Reporting Services
description: "Learn how to use Aspose.Tasks for Java to print reports exported from Microsoft Project (MPP/XML) files."
type: docs
weight: 40
url: /java/reporting-services/
---

{{% alert color="primary" %}} 

Aspose.Tasks provides reporting services for creating reports from project files similar to Microsoft Project. The SaveReport function is used to create PDF files containing the report's images. This function takes two arguments:

1. the PDF file name. and
2. the ReportType enumerator.

{{% /alert %}}

## **Aspose.Tasks Reporting Services**
### **Types of Report**
The following types of reports can be created using Aspose.Tasks:

1. [Project overview](/tasks/java/reporting-services/)
2. [Resource cost overview](/tasks/java/reporting-services/)
3. [Cost overview](/tasks/java/reporting-services/)
4. [Work overview](/tasks/java/reporting-services/)
5. [Critical tasks](/tasks/java/reporting-services/)
6. [Milestones](/tasks/java/reporting-services/)
7. [Late tasks](/tasks/java/reporting-services/)
8. [Resource overview](/tasks/java/reporting-services/)
9. [Cost overruns](/tasks/java/reporting-services/)
10. [Upcoming task](/tasks/java/reporting-services/)
11. [Task cost overview](/tasks/java/reporting-services/)
12. [Over-allocated resources](/tasks/java/reporting-services/)
13. [Slipping tasks](/tasks/java/reporting-services/)
14. [Best practice analyzer](/tasks/java/reporting-services/)
15. [Burn down](/tasks/java/reporting-services/)
16. [Cash flow](/tasks/java/reporting-services/)

The sample code snippets below can be used to create these reports. All the sample MPP files used in these examples are present as attachments for testing the sample code.
#### **Project Overview**
![exported project overview report example Java](reporting-services_1.png)

**Java**

{{< highlight java >}}
Project project = new Project("Cyclic structure.mpp");
project.saveReport("ProjectOverView.pdf", ReportType.ProjectOverview);
{{< /highlight >}}

#### **Resource Cost Overview**
![exported resource cost overview report example Java](reporting-services_2.png)

**Java**

{{< highlight java >}}
Project project = new Project("OzBuild 16 Orig.mpp");
project.saveReport("ResourceCostOverview.pdf", ReportType.ResourceCostOverview);
{{< /highlight >}}

#### **Cost Overview**
![exported cost overview report example Java](reporting-services_3.png)

**Java**

{{< highlight java >}}
Project project = new Project("OzBuild 16 Orig.mpp");
project.saveReport("CostOverview.pdf", ReportType.CostOverview);
{{< /highlight >}}

#### **Work Overview**
![exported work overview report example Java](reporting-services_4.png)

**Java**

{{< highlight java >}}
Project project = new Project("Residential Construction.mpp");
project.saveReport("WorkOverview.pdf", ReportType.WorkOverview);
{{< /highlight >}}

#### **Critical Tasks**

![exported critical tasks report example Java](reporting-services_5.png)

**Java**

{{< highlight java >}}
Project project = new Project("Residential Construction.mpp");
project.saveReport("CriticalTasks.pdf", ReportType.CriticalTasks);
{{< /highlight >}}

#### **Milestones**

![exported milestones report example Java](reporting-services_6.png)

**Java**

{{< highlight java >}}
Project project = new Project("Residential Construction.mpp");
project.saveReport("Milestones.pdf", ReportType.Milestones);
{{< /highlight >}}

#### **Late Tasks**
![exported late tasks report example Java](reporting-services_7.png)

**Java**

{{< highlight java >}}
Project project = new Project("Residential Construction.mpp");
project.saveReport("LateTasks.pdf", ReportType.LateTasks);
{{< /highlight >}}

#### **Resource Overview**
![exported resource overview report example Java](reporting-services_8.png)

**Java**

{{< highlight java >}}
Project project = new Project("Software Development Plan.mpp");
project.saveReport("ResourceOverview.pdf", ReportType.ResourceOverview);
{{< /highlight >}}

#### **Cost Overruns**
![exported cost overruns report example Java](reporting-services_9.png)

**Java**

{{< highlight java >}}
Project project = new Project("Software Development.mpp");
project.saveReport("CostOverruns.pdf", ReportType.CostOverruns);
{{< /highlight >}}

#### **Upcoming Task**
![exported upcoming task report example Java](reporting-services_10.png)

**Java**

{{< highlight java >}}
Project project = new Project("UpcomingTasks.mpp");
project.saveReport("UpcomingTasks.pdf", ReportType.UpcomingTask);
{{< /highlight >}}

#### **Task Cost Overview**
![exported task cost overview report example Java](reporting-services_11.png)

**Java**

{{< highlight java >}}
Project project = new Project("Software Development.mpp");
project.saveReport("TaskCostOverview.pdf", ReportType.TaskCostOverview);
{{< /highlight >}}

#### **Over-allocated Resources**
![exported over-allocated resources report example Java](reporting-services_12.png)

**Java**

{{< highlight java >}}
Project project = new Project("Software Development Plan.mpp");
project.saveReport("OverAllocatedResources.pdf", ReportType.OverallocatedResources);
{{< /highlight >}}

#### **Slipping Tasks**
![exported slipping report example Java](reporting-services_13.png)

**Java**

{{< highlight java >}}
Project project = new Project("Cyclic structure.mpp");
project.saveReport("SlippingTasks.pdf", ReportType.SlippingTasks);
{{< /highlight >}}

#### **Best Practice Analyzer**
![exported best practice report example Java](reporting-services_14.png)

**Java**

{{< highlight java >}}
Project project = new Project("Cyclic structure.mpp");
project.saveReport("BestPracticeAnalyzer.pdf", ReportType.BestPracticeAnalyzer);
{{< /highlight >}}

#### **Burn Down**
![exported practice analyzer report example Java](reporting-services_15.png)

**Java**

{{< highlight java >}}
Project project = new Project("Cyclic structure.mpp");
project.saveReport("Burndown.pdf", ReportType.Burndown);
{{< /highlight >}}

#### **Cash Flow**
![exported burndown report example Java](reporting-services_16.png)

**Java**

{{< highlight java >}}
Project project = new Project("OzBuild 16 Orig.mpp");
project.saveReport("CashFlow.pdf", ReportType.CashFlow);
{{< /highlight >}}
