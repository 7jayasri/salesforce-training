# Day 6 - SOQL and Apex Triggers
# What is SOQL?
SOQL (Salesforce Object Query Language) is a query language used to retrieve data from Salesforce objects.
It is similar to SQL but designed specifically for Salesforce data.
SOQL is used to:
- Retrieve records
- Filter data
- Access related objects
- Generate reports and automation logic

---
# What is an Apex Trigger?
An Apex Trigger is a piece of Apex code that executes automatically when specific events occur on Salesforce records.
Triggers run:
Before insert
After insert
Before update
After update
Before delete
After delete
Triggers help automate complex business logic based on data changes.

# Why Triggers Are Important?
Triggers allow enterprise systems to:
React automatically to events
Maintain data consistency
Automate business processes
Perform validations and updates
# Difference Between Flow and Trigger
Flow	                    | Apex Trigger              |
------------------------- |---------------------------|
No-code automation        |	Code-based automation     |
Easier to create          |	More complex              |
Best for simple processes |	Best for advanced logic   |
Faster implementation   	|Greater flexibility        |
Limited customization   	|Supports complex operations|
# Difference Between Before Trigger and After Trigger
Before Trigger                      |	After Trigger                             |
------------------------------------|-------------------------------------------|
Executes before data is saved	      |Executes after data is saved               |
Used for validation or modification	|Used for notifications and related actions |
Can change record values            |	Cannot directly modify same record easily | 
Faster for validations              |	Best for post-save actions                |
-------
# College Management System Trigger Use Cases
1. After Student Registration → Send Welcome Email
Trigger Event:
After Insert on Student object
Purpose:
Automatically welcomes new students after successful registration.

2. After Course Becomes Full → Notify Faculty
Trigger Event:

After Update on Course object

Purpose:

Alerts faculty when enrollment reaches maximum capacity.

3. After Attendance Drops Below 75% → Send Warning
Trigger Event:

After Update on Attendance record

Purpose:

Warns students about attendance shortage.

4. After Fee Payment → Generate Receipt
Trigger Event:

After Insert on Payment object

Purpose:

Automatically generates payment confirmation.

5. After Student Profile Update → Update Related Records
Trigger Event:

After Update on Student object

Purpose:

Keeps related information synchronized across the system.

Flow vs Trigger Thinking
1. Simple Email Notification
Preferred:
Flow
Why?
Easy to configure and maintain without coding.

2. Complex Fee Eligibility Check
Preferred:
Apex Trigger
Why?
Requires advanced calculations and multiple conditions.

3. Updating Related Records
Preferred:
Flow
Why?
Simple related record updates can be handled declaratively.

4. External API Integration
Preferred:
Apex Trigger
Why?
External integrations require programming and API handling.

# Query Thinking Examples
Student Queries
Find all students in Course A
Get all students enrolled in Course A.
Find all courses handled by Faculty X
Retrieve all courses assigned to Faculty X.
Find students with attendance below 75%
Show students whose attendance percentage is below 75%.
Find all students from CSE Department
Retrieve students belonging to the CSE department.
Find courses with remaining seats available
Display courses where seats are still available.
Why Enterprise Systems Need Event-Driven Behavior

Enterprise systems handle thousands of activities every day. Event-driven behavior helps systems react automatically whenever important changes occur.
Benefits include:
Faster response time
Reduced manual work
Better automation
Improved consistency
Real-time business processing
Without event-driven systems, businesses would rely heavily on manual operations, leading to delays and errors.

# Reflection

Enterprise systems need automatic reactions to data changes because business processes are interconnected. When one event happens, multiple actions may need to occur immediately.
For example:
Student registration may trigger emails
Payment completion may update balances
Attendance shortage may generate warning
Triggers and automation help businesses operate efficiently and intelligently.

# Reflective Questions
1. Why do systems need triggers?
Triggers help systems automatically react to important data changes and events.

2. Difference between polling and event-driven systems?
Polling continuously checks for updates, while event-driven systems react immediately when events occur.

3. Why are database queries important?
Queries help retrieve and manage business data efficiently.

4. When should Flows be preferred over Triggers?
Flows should be preferred for simple automation and easy maintenance.

5. What problems happen if automation logic becomes too complex?
Complex automation becomes difficult to maintain, debug, and scale.

6. Why should developers think carefully before automating actions?
Poor automation design can create errors, performance issues, and unnecessary complexity.

# Trailhead Modules Completed

Database & .NET Basics
Apex Triggers

# Key Learnings
- Understanding SOQL
-Querying Salesforce data
-Event-driven architecture
-Apex Trigger concepts
-Before vs After Triggers
-Flow vs Trigger comparison
-Enterprise automation thinking
# Screenshots

(Add Trailhead completion screenshots here)

# Conclusion

Day 6 helped in understanding how Salesforce retrieves data using SOQL and reacts to events using Apex Triggers. It also explained how enterprise systems use event-driven automation to improve efficiency, consistency, and business operations.
