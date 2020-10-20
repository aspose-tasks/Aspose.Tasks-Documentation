---
title: Reporting Services
type: docs
weight: 40
url: /java/reporting-services/
---

{{% alert color="primary" %}} 

Aspose.Tasks provides reporting services for creating reports from project files similar to Microsoft Project. The SaveReport function is used to create PDF files containing the report's images. This function takes two arguments:

1. the PDF file name. and
1. the ReportType enumerator.

{{% /alert %}} 
## **Aspose.Tasks Reporting Services**
### **Types of Report**
The following types of reports can be created using Aspose.Tasks:

1. [Project overview](/tasks/java/reporting-services/)
1. [Resource cost overview](/tasks/java/reporting-services/)
1. [Cost overview](/tasks/java/reporting-services/)
1. [Work overview](/tasks/java/reporting-services/)
1. [Critical tasks](/tasks/java/reporting-services/)
1. [Milestones](/tasks/java/reporting-services/)
1. [Late tasks](/tasks/java/reporting-services/)
1. [Resource overview](/tasks/java/reporting-services/)
1. [Cost overruns](/tasks/java/reporting-services/)
1. [Upcoming task](/tasks/java/reporting-services/)
1. [Task cost overview](/tasks/java/reporting-services/)
1. [Over-allocated resources](/tasks/java/reporting-services/)
1. [Slipping tasks](/tasks/java/reporting-services/)
1. [Best practice analyzer](/tasks/java/reporting-services/)
1. [Burn down](/tasks/java/reporting-services/)
1. [Cash flow](/tasks/java/reporting-services/)

The sample code snippets below can be used to create these reports. All the sample MPP files used in these examples are present as attachments for testing the sample code.
#### **Project Overview**
![todo:image_alt_text](reporting-services_1.png)

**Java**

{{< highlight java >}}

 //Project OverView

Project project3 = new Project("Cyclic stucture.mpp");

project3.saveReport("ProjectOverView.pdf", ReportType.ProjectOverview);

{{< /highlight >}}
#### **Resource Cost Overview**
![todo:image_alt_text](reporting-services_2.png)

**Java**

{{< highlight java >}}

 //Resource Cost Overview

Project project4 = new Project("OzBuild 16 Orig.mpp");

project4.saveReport("ResourceCostOverview.pdf", ReportType.ResourceCostOverview);

{{< /highlight >}}
#### **Cost Overview**
![todo:image_alt_text](reporting-services_3.png)

**Java**

{{< highlight java >}}

 //Cost Overview

Project project5 = new Project("OzBuild 16 Orig.mpp");

project5.saveReport("CostOverview.pdf", ReportType.CostOverview);

{{< /highlight >}}
#### **Work Overview**
![todo:image_alt_text](reporting-services_4.png)

**Java**

{{< highlight java >}}

 //Work Overview

Project project6 = new Project("Residential Construction.mpp");

project6.saveReport("WorkOverview.pdf", ReportType.WorkOverview);

{{< /highlight >}}
#### **Critical Tasks**
![todo:image_alt_text](reporting-services_5.png)

**C#**

{{< highlight csharp >}}

 //Critical Tasks

Project project7 = new Project("Residential Construction.mpp");

project7.saveReport("CriticalTasks.pdf", ReportType.CriticalTasks);

{{< /highlight >}}
#### **Milestones**
![todo:image_alt_text](reporting-services_6.png)

**C#**

{{< highlight csharp >}}

 //Milestones

Project project8 = new Project("Residential Construction.mpp");

project8.saveReport("Milestones.pdf", ReportType.Milestones);

{{< /highlight >}}
#### **Late Tasks**
![todo:image_alt_text](reporting-services_7.png)

**C#**

{{< highlight csharp >}}

 //Late Tasks

Project project9 = new Project("Residential Construction.mpp");

project9.saveReport("LateTasks.pdf", ReportType.LateTasks);

{{< /highlight >}}
#### **Resource Overview**
![todo:image_alt_text](reporting-services_8.png)

**C#**

{{< highlight csharp >}}

 //Resource Overview

Project project10 = new Project("Software Development Plan.mpp");

project10.saveReport("ResourceOverview.pdf", ReportType.ResourceOverview);

{{< /highlight >}}
#### **Cost Overruns**
![todo:image_alt_text](reporting-services_9.png)

**C#**

{{< highlight csharp >}}

 //Cost Overruns

Project project11 = new Project("Software Development.mpp");

project11.saveReport("CostOverruns.pdf", ReportType.CostOverruns);

{{< /highlight >}}
#### **Upcoming Task**
![todo:image_alt_text](reporting-services_10.png)

**C#**

{{< highlight csharp >}}

 //Upcoming Task

Project project12 = new Project("UpcomingTasks.mpp");

project12.saveReport("UpcomingTasks.pdf", ReportType.UpcomingTask);

{{< /highlight >}}
#### **Task Cost Overview**
![todo:image_alt_text](reporting-services_11.png)

**C#**

{{< highlight csharp >}}

 //Task Cost Overview

Project project13 = new Project("Software Development.mpp");

project13.saveReport("TaskCostOverview.pdf", ReportType.TaskCostOverview);

{{< /highlight >}}
#### **Over-allocated Resources**
![todo:image_alt_text](reporting-services_12.png)

**C#**

{{< highlight csharp >}}

 //Over allocated Resources

Project project14 = new Project("Software Development Plan.mpp");

project14.saveReport("OverAllocatedResources.pdf", ReportType.OverallocatedResources);

{{< /highlight >}}
#### **Slipping Tasks**
![todo:image_alt_text](reporting-services_13.png)

**C#**

{{< highlight csharp >}}

 //Slipping Tasks

Project project15 = new Project("Cyclic stucture.mpp");

project15.saveReport("SlippingTasks.pdf", ReportType.SlippingTasks);

{{< /highlight >}}
#### **Best Practice Analyzer**
![todo:image_alt_text](reporting-services_14.png)

**C#**

{{< highlight csharp >}}

 //Best Practice Analyzer

Project project16 = new Project("Cyclic stucture.mpp");

project16.saveReport("BestPracticeAnalyzer.pdf", ReportType.BestPracticeAnalyzer);

{{< /highlight >}}
#### **Burn Down**
![todo:image_alt_text](reporting-services_15.png)

**C#**

{{< highlight csharp >}}

 //Burn down

Project project17 = new Project("Cyclic stucture.mpp");

project17.saveReport("Burndown.pdf", ReportType.Burndown);

{{< /highlight >}}
#### **Cash Flow**
![todo:image_alt_text](reporting-services_16.png)

**C#**

{{< highlight csharp >}}

 //Cash Flow

Project project18 = new Project("OzBuild 16 Orig.mpp");

project18.saveReport("CashFlow.pdf", ReportType.CashFlow);

{{< /highlight >}}
