---
title: Verifying Project Structure in Ruby
type: docs
weight: 150
url: /java/verifying-project-structure-in-ruby/
---

## **Aspose.Tasks - Verifying Project Structure**
To Verify Project Structure using **Aspose.Tasks Java for Ruby**, simply invoke **VerifyProjectStructure** module. Here you can see example code.

**Ruby Code**

{{< highlight ruby >}}

 data_dir = File.dirname(File.dirname(File.dirname(File.dirname(__FILE__)))) + '/data/'



\# Instantiate project object

project = Rjb::import('com.aspose.tasks.Project').new(data_dir + 'test_tasks.mpp')

if project.check()

    puts "Project is ok"

else

    puts "Project is not ok"

end

{{< /highlight >}}
## **Download Running Code**
Download **Verifying Project Structure (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_Ruby/lib/asposetasksjava/Projects/verifyprojectstructure.rb)
