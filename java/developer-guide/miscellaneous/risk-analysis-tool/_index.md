---
title: Risk Analysis Tool
type: docs
weight: 50
url: /java/risk-analysis-tool/
---

## **Performing Risk Analysis**
Aspose.Tasks API supports for performing risk analysis on a Project data file. This is based on the Monte Carlo simulation that supports different probability distributions and correlations. The [RiskAnalyzer](http://www.aspose.com/api/java/tasks/com.aspose.tasks/classes/RiskAnalyzer) class can be used to perform the risk analysis that is based on a project schedule (task durations and their start/finish dates). So, a project Finish date can be the output of such analysis. The following example illustrates this functionality step-by-step.
### **1. Preparing Analysis Settings**
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Miscellaneous-RiskAnalyzerTest-prepare-risk-analysis.java" >}}
### **2. Identifying the Input of Analysis**
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Miscellaneous-RiskAnalyzerTest-identify-input-of-analysis.java" >}}
### **3. Analyze the Risks**
**Java**

{{< highlight java >}}

 RiskAnalyzer analyzer = new RiskAnalyzer(settings);

RiskAnalysisResult analysisResult = analyzer.analyze(project);

{{< /highlight >}}
### **4. Use the Results of the Analysis**
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Miscellaneous-RiskAnalyzerTest-use-analysis.java" >}}
