logic to save inference and make it super efficient.

\### Abstract: ADCLPS Low-Cost School KPI Logic



ADCLPS is a simple tracking logic where every domain is broken into small measurable actions called sub-KPIs.



Example domains:



Discipline

Faith

Love



Each domain can have 20 sub-KPIs.



Instead of storing long text every time, the system stores only the needed value.



Example:



D5 means Discipline sub-KPI number 5 is completed.



So the system does not need to store:



“Student completed discipline task number 5”



It only stores:



D5



This saves:



Data storage

Data transfer

Inference cost

Processing cost

User input time



\### Simple Data Logic



Each entry records only:



Domain code

Mark

Time

Class

User ID



Example:



Discipline, X, 9 AM, Class 2, C2SBK



Meaning:



A student from Class 2 completed or was marked for a discipline KPI at 9 AM.



\### User ID Logic



Example:



C6SBH



Means:



C6 = Class 6

SB = Section B

H = Hero / student name code



So one small code can identify the student without writing full details again and again.



\### KPI Completion Logic



Example:



D5

D16

D12



Means:



Out of 20 Discipline KPIs, KPI number 5, 16, and 12 are completed.



The system can calculate:



Completed KPIs

Pending KPIs

Low consistency

Mid consistency

High consistency

Class performance

Student performance

Domain performance



\### UI Logic



The input form should always be in simple words.



Example:



Select Domain: Discipline

Select KPI: Cleanliness

Mark: Done or Not Done

Select Class: Class 6

Select Section: B

Select Student: Hero



The system can convert it into:



D5, X, 9 AM, C6SBH



So users see simple words, but the database stores short codes.



\### Core Benefit



ADCLPS keeps the front side simple for humans and the back side efficient for machines.



Users enter words.



The system stores codes.



Dashboards are calculated from small marks.



This makes the website fast, lightweight, low-cost, easy to use, and suitable for HTML, CSS, JavaScript, and SQL.



