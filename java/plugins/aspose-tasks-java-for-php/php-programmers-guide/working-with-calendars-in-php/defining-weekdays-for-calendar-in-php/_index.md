---
title: Defining Weekdays for Calendar in PHP
type: docs
weight: 20
url: /java/defining-weekdays-for-calendar-in-php/
---

## **Aspose.Tasks - Defining Weekdays for Calendar**
To Define Weekdays for Calendar using **Aspose.Tasks Java for PHP**, simply invoke **DefineWeekdaysForCalendar** module. Here you can see example code.

{{< highlight php >}}
$project = new Project();
$cal = $project->getCalendars()->add("Calendar1");
$weekday = new WeekDay();
$dayType = new DayType();
$cal->getWeekDays()->add($weekday->createDefaultWorkingDay($dayType->Monday));
$cal->getWeekDays()->add($weekday->createDefaultWorkingDay($dayType->Tuesday));
$cal->getWeekDays()->add($weekday->createDefaultWorkingDay($dayType->Wednesday));
$cal->getWeekDays()->add($weekday->createDefaultWorkingDay($dayType->Thursday));
$cal->getWeekDays()->add(new WeekDay($dayType->Saturday));
$cal->getWeekDays()->add(new WeekDay($dayType->Sunday));
$myWeekDay = new WeekDay($dayType->Friday);
$wt1 = new WorkingTime();
$calendar = new Calendar();
$calTime = $calendar->getInstance();
$calTime->set(1,1,1,9,0,0);
$date = $calTime->getTime();
$time1->setFromTime($date);
$calTime->set(1,1,1,12,0,0);
$date = $calTime->getTime();
$time1->setToTime($date);
$time2 = new WorkingTime();
$calTime->set(1,1,1,13,0,0);
$date = $calTime->getTime();
$time2->setFromTime($date);
$calTime->set(1,1,1,16,0,0);
$date = $calTime->getTime();
$time2->setToTime($date);
$myWeekDay->getWorkingTimes()->add($time1);
$myWeekDay->getWorkingTimes()->add($time2);
$myWeekDay->setDayWorking(true);
$cal->getWeekDays()->add($myWeekDay);
$saveFileFormat = new SaveFileFormat();
$project->save("CalendarWeekdays.xml", $saveFileFormat->XML);
print "Defined weekdays for calendar, please check the output file.".PHP_EOL;
{{< /highlight >}}

## **Download Running Code**
Download **Defining Weekdays for Calendar (Aspose.Tasks)** from any of the below mentioned social coding sites:

- [GitHub](https://github.com/aspose-tasks/Aspose.Tasks-for-Java/blob/master/Plugins/Aspose_Tasks_Java_for_PHP/src/aspose/tasks/WorkingWithCalendars/DefineWeekdaysForCalendar.php)
