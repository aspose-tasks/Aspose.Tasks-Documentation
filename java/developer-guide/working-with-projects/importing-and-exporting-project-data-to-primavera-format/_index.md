---
title: Importing and Exporting Project Data to Primavera Format
type: docs
weight: 60
url: /java/importing-and-exporting-project-data-to-primavera-format/
---

{{% alert color="primary" %}} 

Primavera’s Proprietary Exchange Format (XER), by Primavera Systems, Inc., is primarily associated with Primavera Project Management. Aspose.Tasks provides the capability to export Microsoft Project Data to Primavera XER and XML formats. This article shows how to export project data to both these formats. 

{{% /alert %}} 

## **Importing Data from Primavera File**

### **Importing Data from Primavera XML Format**
Aspose.Tasks can import *Primavera* XML similar to Microsoft Project XML and MPP formats. The Project class provides the capability of loading such type of file using the same constructor as used for other Project files.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ImportExportDataToPrimavera-import-data-from-primavera-xml-format.java" >}}

### **Importing Data from Primavera MPX File Format**

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ImportExportDataToPrimavera-import-data-from-primavera-mpx-format.java" >}}

### **Reading Project UIDs from Primavera XML file**
A Primavera XML file may contain multiple projects, each having its own UID. Aspose.Tasks for Java API provides the capability to read all such UIDs from the project and then load a project using a specific id from the list of UIDs.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ImportExportDataToPrimavera-read-all-project-uid.java" >}}

### **Reading Primavera XML file with Multiple Projects**
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ImportExportDataToPrimavera-read-project-specific-uid.java" >}}

## **Importing Project Data from Primavera Database File**
{{< highlight java >}}
String url = "jdbc:sqlserver://";
String serverName = "192.168.56.3\\MSSQLSERVER";
String portNumber = "1433";
String databaseName = "PrimaveraEDB";
String userName = "privuser";
String password = "***";
PrimaveraDbSettings settings = new PrimaveraDbSettings(url+serverName + ":" + portNumber + ";databaseName=" + databaseName + ";user=" + userName + ";password=" + password, 4502);
// set driver name
settings.setDriverClassName("com.microsoft.sqlserver.jdbc.SQLServerDriver");
// note that you have to set the classpath to include the sqljdbc.jar file or the sqljdbc4.jar file, otherwise  "Class not found" exception will be thrown
// here we add classpath dynamically just for testing needs:
addJDBCDriver(new File("c:\\Program Files (x86)\\Microsoft JDBC Driver 4.0 for SQL Server\\sqljdbc_4.0\\enu\\sqljdbc4.jar"));
Project project = new Project(settings);
private static void addJDBCDriver(File file) throws Exception
{
    Method method = URLClassLoader.class.getDeclaredMethod("addURL", new Class[]{URL.class});
    method.setAccessible(true);
    method.invoke(ClassLoader.getSystemClassLoader(), new Object[]{file.toURI().toURL()});
}
{{< /highlight >}}

## **Support for SQLite Database**
{{< highlight java >}}
const string connectionString = "Data Source=d:\\DB\\PPMDBSQLite.db";
const int projectId = 4502;
PrimaveraDbSettings primaveraDbSettings = new PrimaveraDbSettings(connectionString, projectId);
primaveraDbSettings.setProviderInvariantName("System.Data.SQLite");
Project project = new Project(primaveraDbSettings);
{{< /highlight >}}

## **Exporting Project Data in Primavera Formats**
The SaveFileFormat enumerator is used to specify the project export type as Primavera XML or XER.
### **Exporting Project Data to Primavera XML Format**
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ImportExportDataToPrimavera-export-data-to-primavera-xml-format.java" >}}
### **Exporting Project Data to Primavera XER Format**
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ImportExportDataToPrimavera-export-data-to-primavera-xer-format.java" >}}
### **Exporting Project Data to Primavera MPX Format**
{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ImportExportDataToPrimavera-export-data-to-primavera-mpx-format.java" >}}
### **Primavera XML Save Options**
If Primavera XML file doesn't has any WBS inside (only Activities), Aspose.Tasks can't read properly this type of file, because the API needs a root task to create a tree of tasks.
In this case, the API creates a RootTask, even if it doesn't exist in the file, to be able to read these particular files. If the user wants to save after reading, it'll be saving with created RootTask, which did not exist before reading. This option helps to decide how to save into the file - with created RootTask or not. By default, it set to true.

{{< gist "aspose-com-gists" "472405ac9bab4502a485ee007b92074c" "Examples-src-main-java-com-aspose-tasks-examples-Projects-ImportExportDataToPrimavera-primavera-xml-save-options.java" >}}
