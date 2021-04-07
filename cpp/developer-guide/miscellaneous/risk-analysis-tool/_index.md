---
title: Risk Analysis Tool
description: "Learn how to use risk analysis tools to perform risk analysis on Microsoft Project (MPP/XML) files using Aspose.Tasks for C++."
type: docs
weight: 40
url: /cpp/risk-analysis-tool/
---

## **Performing Risk Analysis**
Aspose.Tasks for C++ API supports performing risk analysis on Microsoft Project files. This is based on the Monte Carlo simulation that supports different probability distributions and correlations. The Aspose.Tasks.RiskAnalysis.RiskAnalyzer class can be used to perform the risk analysis that is based on a project schedule (task durations and their start/finish dates). So, a project Finish date can be the output of such analysis. The following code example illustrates this functionality step-by-step.

### **Preparing Analysis Settings**

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-Miscellaneous-PerformRiskAnalysis-PrepareAnalysisSettings.cpp" >}}

### **Identifying the Input of Analysis**

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-Miscellaneous-PerformRiskAnalysis-IdentifyAnalysisInput.cpp" >}}

{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-Miscellaneous-PerformRiskAnalysis-AnalyzeRisks.cpp" >}}

### **Use the Results of the Analysis**
{{< gist "aspose-com-gists" "85d3cb818a62006b9ae8f8e3eaab6f80" "Examples-CPP-Miscellaneous-PerformRiskAnalysis-UseAnalysisResult.cpp" >}}
