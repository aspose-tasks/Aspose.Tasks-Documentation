---
title: Aspose.Tasks Java For PHP
description: "This page contains an introduction to Aspose.Tasks Java for PHP."
type: docs
weight: 40
url: /java/aspose-tasks-java-for-php/
---

## **Introduction to Aspose.Tasks Java for PHP**

Aspose.Tasks Java for PHP is created using [PHP / Java Bridge](http://php-java-bridge.sourceforge.net/pjb/). The PHP/Java Bridge is an implementation of a streaming, XML-based [network protocol](http://php-java-bridge.sourceforge.net/pjb/PROTOCOL.TXT), which can be used to connect a native script engine, for example PHP, Scheme or Python, with a Java virtual machine. It is up to 50 times faster than local RPC via SOAP, requires less resources on the web-server side. It is [faster](http://php-java-bridge.sourceforge.net/pjb/FAQ.html#performance) and more reliable than direct communication via the Java Native Interface, and it requires no additional components to invoke Java procedures from PHP or PHP procedures from Java.

Read more at [sourceforge.net](http://php-java-bridge.sourceforge.net/pjb/)

## **Aspose.Tasks for Java**
Aspose.Tasks for Java is a project management API that enables Java application developers to provide MPP/P6XML document manipulation capability in their applications – all without using Microsoft Project. With this powerful API, developers can control various stages of project management, such as project planning, definition and tracking.

## **Aspose.Tasks Java for PHP**
Project Aspose.Tasks for PHP shows how different tasks can be performed using Aspose.Tasks Java APIs in PHP. This project is aimed to provide useful examples for PHP Developers who want to utilize Aspose.Tasks for Java in their PHP Projects using [PHP/Java Bridge](https://sourceforge.net/projects/php-java-bridge/files/Binary%20package/php-java-bridge_7.2.1/php-java-bridge_7.2.1_documentation.zip/download).

## **System Requirements**

**Following are the system requirements to use Aspose.Tasks Java for PHP:**

- Tomcat Server 8.0 or above installed.
- PHP/JavaBridge is configured.
- FastCGI is installed.
- Downloaded Aspose.Tasks component.

## **Supported Platforms**
**Following are the supported platforms:**

- PHP 5.3 or above
- Java 1.8 or above

## **Download Required Libraries**
Download required libraries mentioned below. These are the required for executing Aspose.Tasks Java for PHP examples.

- **Aspose:** [Aspose.Tasks for Java Component](https://downloads.aspose.com/tasks/net)
- [PHP/Java Bridge](https://sourceforge.net/projects/php-java-bridge/files/Binary%20package/php-java-bridge_7.2.1/php-java-bridge_7.2.1_documentation.zip/download)

## **Download Examples from Social Coding Sites**
Following releases of running examples are available to download on:
- [Aspose.Tasks Java for PHP](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/tree/master/Plugins/Aspose_Tasks_Java_for_PHP)

## **How to configure the source code on Linux Platform**
Please follow these simple steps in order to open and extend the source code while using:

## **1. Install Tomcat Server**
To install tomcat server, issue following command on the linux console. This will successfully install tomcat server. 

{{< highlight text >}}
sudo apt-get install tomcat8
{{< /highlight >}}

## **2. Download and Configure PHP/JavaBridge**
In order to download the PHP/JavaBridge binaries, issue following command on the linux console. 

{{< highlight text >}}
wget https://citylan.dl.sourceforge.net/project/php-java-bridge/Binary%20package/php-java-bridge_6.2.1/php-java-bridge_6.2.1_documentation.zip 
{{< /highlight >}}

Unzip the PHP/JavaBridge binaries by issuing the following command on linux console. 

{{< highlight text >}}
unzip -d php-java-bridge_6.2.1_documentation.zip 
{{< /highlight >}}

This will extract **JavaBridge.war** file. Copy it to tomcat88 **webapps** folder by issuing the following command on Linux console. 

{{< highlight text >}}
sudo cp JavaBridge.war /var/lib/tomcat8/webapps/JavaBridge.war 
{{< /highlight >}}

By copying, tomcat8 will automatically create a new folder "**JavaBridge**" in **webapps**. Once the folder is created, make sure your tomcat8 is running and then check <https://localhost:8080/JavaBridge> in browser, it should open a default page of JavaBridge. 

If any error message appears then install  **FastCGI** by issuing the following command on Linux console.

{{< highlight text >}}
sudo apt-get install php55-cgi 
{{< /highlight >}}

After installing php5.5 CGI, restart tomcat8 server and check <https://localhost:8080/JavaBridge> again in the browser.

If **JAVA_HOME** error is displayed, then open /etc/default/tomcat8 file and uncomment the line that sets the JAVA_HOME. Check <https://localhost:8080/JavaBridge> in browser again, it should come with PHP/JavaBridge Examples page.

## **3. Configure Aspose.Tasks Java for PHP Examples**
Clone, PHP examples by issuing the following commands inside webapps/JavaBridge folder.  

{{< highlight text >}}
git init
git clone [https://github.com/asposeslides/Aspose_Slides_Java/tree/master/Plugins/Aspose_Tasks_Java_for_PHP] 
{{< /highlight >}}

## **How to configure the source code on Windows Platform**
Please follow below simple steps to configure PHP/Java Bridge on Windows Platform

1. Install PHP5 and configure as you normally do
2. Install JRE 6 (Java Runtime Environment) if you don’t already have it. You can check this in C:\Program Files etc. You can download it here . I am using JRE 6 as It is compatible with PHP Java Bridge (PJB).
3. Install Apache Tomcat 8.0. You can download it here
4. Download [JavaBridge.war](https://sourceforge.net/projects/php-java-bridge/files/Binary%20package/php-java-bridge_7.2.1/JavaBridgeTemplate721.war/download). Copy this file to tomcat webapps directory.
(ex: C:\Program Files\Apache Software Foundation\Tomcat 8.0\webapps )
5. Restart tomcat apache service.
6. Go to <http://localhost:8080/JavaBridge/test.php> to check if php works. You can find other examples in there
7. Copy your [Aspose.Tasks Java](https://downloads.aspose.com/tasks/java) jar file to C:\Program Files\Apache Software Foundation\Tomcat 8.0\webapps\JavaBridge\WEB-INF\lib
8. Clone [Aspose.Tasks Java for PHP](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/tree/master/Plugins/Aspose_Tasks_Java_for_PHP) examples inside C:\Program Files\Apache Software Foundation\Tomcat 8.0\webapps\ folder.
9. Copy folder C:\Program Files\Apache Software Foundation\Tomcat 8.0\webapps\JavaBridge\java to your Aspose.Tasks Java for PHP examples folder.
10. Restart apache tomcat service and start using examples.
