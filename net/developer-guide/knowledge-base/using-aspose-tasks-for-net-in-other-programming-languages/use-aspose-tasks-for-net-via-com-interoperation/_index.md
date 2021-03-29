---
title: Use Aspose.Tasks for .NET via COM Interoperation
type: docs
weight: 20
url: /net/use-aspose-tasks-for-net-via-com-interoperation/
---

{{% alert color="primary" %}} 

The information in this topic applies to scenarios where you want to use Aspose.Tasks for .NET via COM Interop in any of the following programming languages:

- Visual Basic 6
- ASP Classic with VB Script

{{% /alert %}} 
## **Working with COM Interop**
Aspose.Tasks for .NET executes under the control of the .NET Framework and this is called managed code. Code written in all of the above languages runs outside the .NET Framework and it is called unmanaged code. Interaction between unmanaged code and Aspose.Tasks occurs via the .NET facility called COM Interop.

Aspose.Tasks objects are .NET objects, but when used via COM Interop, they appear as COM objects in your programming language. Therefore, it is best to make sure you know how to create and use COM objects in your programming language, before you start using Aspose.Tasks.

Here are the topics that you will eventually need to master:

- Using COM objects in your programming language. See your programming language documentation and the language-specific topics further in this documentation.
- Working with COM objects exposed by .NET COM Interop. See [Interoperating With Unmanaged Code](http://msdn.microsoft.com/en-us/library/sd10k43k.aspx) and [Exposing .NET Framework Components to COM](http://msdn.microsoft.com/en-us/library/zsfww439%28v=vs.110%29.aspx) in MSDN.
- The Aspose.Tasks document object model. See Aspose.Tasks [Developer Guide](/tasks/net/developer-guide/) and [API Reference](http://www.aspose.com/api/net/tasks).
### **Register Aspose.Tasks for .NET with COM Interop**
You need to install Aspose.Tasks for .NET and make sure that it is registered with COM Interop (ensuring that it can be called from unmanaged code).

1. Aspose.Tasks for COM Interop can be registered by executing the following command:
   regasm "C:\Program Files\Aspose\Aspose.Tasks\bin\net20\Aspose.Tasks.DLL" /codebase
2. Now, the COM type library can be exported in the same directory using the following command:
   regasm "<directory>" /tlb:Aspose.Tasks.tlb

regasm.exe is a tool included in .NET Framework SDK. All the .NET Framework SDK tools are located in the **\Microsoft .NET\Framework\<FrameworkVersion>** directory. It will run a command prompt with all the necessary environment variables set.

If your programming language (for example, Visual Basic) allows you to reference a COM type library, then add a reference to Aspose.Tasks.tlb and you will be able to see all Aspose.Tasks classes, methods, properties and enumerations in your Object Browser.

Once created, you are able to access the object’s methods and properties, as if it was a COM object:



{{< highlight java >}}

 Dim prj As New Aspose_Tasks.Project

prj.IsScheduleFromStart = True

{{< /highlight >}}

{{% alert color="primary" %}} 

Some methods have overloads and they will be exposed by COM Interop with a numeric suffix added to them, except for the very first method that stays unchanged. For example, Project.CalcCalendarUids method overloads become Project.CalcCalendarUids, Project.CalcCalendarUids _2 and so on.

{{% /alert %}}
