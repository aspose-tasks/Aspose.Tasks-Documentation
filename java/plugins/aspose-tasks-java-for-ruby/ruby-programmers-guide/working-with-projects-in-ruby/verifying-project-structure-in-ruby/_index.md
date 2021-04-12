---
title: Verifying Project Structure in Ruby
description: "Learn how to verify Microsoft Project (MPP/XML) project structure using Aspose.Tasks Java for Ruby."
type: docs
weight: 150
url: /java/verifying-project-structure-in-ruby/
---

## **Aspose.Tasks - Verifying Project Structure**
To Verify Project Structure using **Aspose.Tasks Java for Ruby**, simply invoke **VerifyProjectStructure** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}
project = Rjb::import('com.aspose.tasks.Project').new('test_tasks.mpp')
if project.check()
    puts "Project is ok"
else
    puts "Project is not ok"
end
{{< /highlight >}}

## **Download Running Code**
Download **Verifying Project Structure (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/verifyprojectstructure.rb)
