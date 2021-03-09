---
title: Defining Weekdays for Calendar in PHP
type: docs
weight: 20
url: /java/defining-weekdays-for-calendar-in-php/
---

## **Aspose.Tasks - Defining Weekdays for Calendar**
To Define Weekdays for Calendar using **Aspose.Tasks Java for PHP**, simply invoke **DefineWeekdaysForCalendar** module. Here you can see example code.

**PHP Code**

{{< highlight php >}}

 # Instantiate project object

$project = new Project();

\# Define Calendar

$cal = $project->getCalendars()->add("Calendar1");

$weekday = new WeekDay();

$daytype = new DayType();

\# Add working days monday through thursday with default timings

$cal->getWeekDays()->add($weekday->createDefaultWorkingDay($daytype->Monday));

$cal->getWeekDays()->add($weekday->createDefaultWorkingDay($daytype->Tuesday));

$cal->getWeekDays()->add($weekday->createDefaultWorkingDay($daytype->Wednesday));

$cal->getWeekDays()->add($weekday->createDefaultWorkingDay($daytype->Thursday));

$cal->getWeekDays()->add(new WeekDay($daytype->Saturday));

$cal->getWeekDays()->add(new WeekDay($daytype->Sunday));

\# Set friday as short working day

$myWeekDay = new WeekDay($daytype->Friday);

\# Sets working time. Only time part of DateTime is important

$wt1 = new WorkingTime();

$calendar=new Calendar();

$calTime = $calendar->getInstance();

$calTime->set(1,1,1,9,0,0);

$date = $calTime->getTime();

$wt1->setFromTime($date);

$calTime->set(1,1,1,12,0,0);

$date = $calTime->getTime();

$wt1->setToTime($date);

$wt2 = new WorkingTime();

$calTime->set(1,1,1,13,0,0);

$date = $calTime->getTime();

$wt2->setFromTime($date);

$calTime->set(1,1,1,16,0,0);

$date = $calTime->getTime();

$wt2->setToTime($date);

$myWeekDay->getWorkingTimes()->add($wt1);

$myWeekDay->getWorkingTimes()->add($wt2);

$myWeekDay->setDayWorking(true);

$cal->getWeekDays()->add($myWeekDay);

\# Save the Project

$saveFileFormat=new SaveFileFormat();

$project->save($dataDir . "CalendarWeekdays.xml", $saveFileFormat->XML);

print "Defined weekdays for calendar, please check the output file.".PHP_EOL;


{{< /highlight >}}
## **Download Running Code**
Download **Defining Weekdays for Calendar (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithCalendars/DefineWeekdaysForCalendar.php)
