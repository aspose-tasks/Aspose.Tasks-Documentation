---
title: Installation
type: docs
weight: 40
url: /java/installation/
---

## **Installing Aspose.Tasks for Java**
Aspose hosts all Java APIs on [Aspose Artifactory](https://repository.aspose.com/webapp/#/home). You can easily use [Aspose.Tasks for Java](https://repository.aspose.com/webapp/#/artifacts/browse/tree/General/repo/com/aspose/aspose-tasks) API directly in your Maven Projects with simple configurations.
### **Specify Maven Repository Configuration**
First, you need to specify the Aspose Maven Repository configuration/location in your Maven pom.xml as follows:

{{< highlight java >}}

 <repositories>

    <repository>

        <id>AsposeJavaAPI</id>

        <name>Aspose Java API</name>

        <url>http://repository.aspose.com/repo/</url>

    </repository>

</repositories>

{{< /highlight >}}
### **Define Aspose.Tasks for Java API Dependency**
Then define Aspose.Tasks for Java API dependency in your pom.xml as follows:

{{< highlight java >}}

 <dependency>

    <groupId>com.aspose</groupId>

    <artifactId>aspose-tasks</artifactId>

    <version>20.4</version>

    <classifier>jdk17</classifier>

</dependency>

{{< /highlight >}}

After performing the above steps, Aspose.Tasks for Java dependency will finally be defined in your Maven Project.
