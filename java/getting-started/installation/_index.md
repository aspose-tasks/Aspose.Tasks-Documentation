---
title: Installation of Aspose.Tasks for Java
description: "Learn how to install Aspose.Tasks for Java via Aspose Artifactory."
type: docs
weight: 40
url: /java/installation/
---

## **Installing Aspose.Tasks for Java**
Aspose hosts all Java APIs on [Aspose Artifactory](https://releases.aspose.com/java/repo/). You can easily use [Aspose.Tasks for Java](https://repository.aspose.com/java/repo/com/aspose/aspose-tasks) API directly in your Maven Projects with simple configurations.

### **Specify Maven Repository Configuration**
First, you need to specify the Aspose Maven Repository configuration/location in your Maven pom.xml as follows:

{{< highlight text >}}
<repositories>
   <repository>
       <id>AsposeJavaAPI</id>
       <name>Aspose Java API</name>
       <url>https://releases.aspose.com/java/repo/</url>
   </repository>
</repositories>
{{< /highlight >}}

### **Define Aspose.Tasks for Java API Dependency**
Then define Aspose.Tasks for Java API dependency in your pom.xml as follows:

{{< highlight text >}}
<dependency>
   <groupId>com.aspose</groupId>
   <artifactId>aspose-tasks</artifactId>
   <version>20.10</version>
   <classifier>jdk18</classifier>
</dependency>
{{< /highlight >}}

After performing the above steps, Aspose.Tasks for Java dependency will finally be defined in your Maven Project.
