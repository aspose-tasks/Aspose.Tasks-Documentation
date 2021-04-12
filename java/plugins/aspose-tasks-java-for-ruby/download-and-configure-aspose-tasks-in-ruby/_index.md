---
title: Download and Configure Aspose.Tasks in Ruby
description: "Learn how to configure Aspose.Tasks Java for Ruby."
type: docs
weight: 10
url: /java/download-and-configure-aspose-tasks-in-ruby/
---

## **Download Required Libraries**
Download required libraries mentioned below. These are the required for executing Aspose.Tasks Java for Ruby examples.

- [Aspose.Tasks for Java Component](https://downloads.aspose.com/tasks/java)

## **Download Examples from Social Coding Sites**
Following releases of running examples are available to download on below mentioned social coding sites:

**GitHub**

- [Aspose.Tasks Java for Ruby](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/tree/master/Plugins/Aspose_Tasks_Java_for_Ruby)

## **Installing**
It is very simple and easy to install Aspose.Tasks Java for Ruby gem, please follow these simple steps:

1. Run following command.

{{< highlight ruby >}}
$ gem install aspose-tasksjava
{{< /highlight >}}

1. Download required Aspose.Tasks for Java Component from following link.
   <https://downloads.aspose.com/tasks/java>
2. Create "jars" folder at root of the Aspose.Tasks Java for Ruby gem and copy downloaded component into it.

## **Using**
Include the required files to get project version.

{{< highlight ruby >}}
require File.dirname(File.dirname(File.dirname(__FILE__))) + '/lib/aspose-tasksjava'
include Asposetasksjava
include Asposetasksjava::ProjectVersion
initialize_aspose_tasks
{{< /highlight >}}

Let's understand the above code.

1. The first line makes sure that the Aspose.Tasks is loaded and available.
2. Include the files that are required to access the Aspose.Tasks.
3. Initialize the libraries. The aspose JAVA classes are loaded from the path provided in the aspose.yml file
