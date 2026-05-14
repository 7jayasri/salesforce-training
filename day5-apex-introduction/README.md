# Day 5 - Apex Introduction


# What is Apex?
Apex is a strongly typed programming language developed by Salesforce that allows developers to add custom business logic to Salesforce applications.
It is similar to Java and is used for:
- Advanced automation
- Custom validations
- Database operations
- Integrations
- Complex business logic
Apex runs on the Salesforce platform and works closely with Salesforce objects and data.

---

# Why Apex is Needed
Salesforce provides no-code tools like Flows and Validation Rules, but some business requirements become too complex for declarative tools alone.
Apex is needed when:
- Logic becomes highly complex
- External integrations are required
- Advanced calculations are needed
- Large-scale automation is required

---

# Difference Between Flow and Apex

| Flow | Apex |
|--------------------------------|------------------------------------------|
| No-code automation             | Programming-based automation             |
| Easy to build                  | Requires coding knowledge                |
| Best for simple processes      | Best for complex logic                   |
| Faster development             | More flexible and powerful               |
| Limited advanced customization | Supports advanced customization          |

---

# Difference Between Configuration and Coding

| Configuration                  | Coding                           |
|--------------------------------|----------------------------------|
| Built using clicks             | Built using programming          |
| Faster implementation          | More customization               |
| Easier maintenance             | Handles advanced requirements    |
| Best for simple business rules | Best for complex business logic  |

---

# College Management System Integration
## CRM
The CRM system manages student admissions, courses, faculty, and communication.
---
# Objects Used
1. Student
2. Faculty
3. Course
4. Department

---
# Relationships

| Parent Object | Child Object | Relationship |
|---------------|--------------|--------------|
| Department    | Faculty      | Lookup       |
| Department    | Course       | Lookup       |
| Course        | Student      | Lookup       |

Relationships help organize and connect business data efficiently.
---

# Validation Rules
## Example:
Student email cannot be blank.
### Purpose:
Prevents incomplete student records from being saved.

---

# Formula Fields
## Example:
Remaining Seats = Total Seats - Enrolled Students
### Purpose:
Automatically calculates available seats.

---

# Flows

## Example:
Auto email notification after student registration.

### Purpose:
Improves communication and reduces manual work.

---

# Apex Usage

## Example:
Advanced student eligibility calculation for scholarship approval.

### Purpose:
Implements complex business logic that Flow cannot easily handle.

---

# Real Examples Where Apex is Needed

## 1. Complex Fee Calculation
### Scenario:
Calculate fees based on scholarship percentage, attendance, and course type.
### Why Apex?
The logic becomes too complex for simple Flow conditions.

---
## 2. External Payment Gateway Integration
### Scenario:
Connect Salesforce with an external payment system.
### Why Apex?
API integration and custom request handling require programming.

---
## 3. Advanced Eligibility Verification
### Scenario:
Check multiple conditions before approving admission.
### Conditions:
- Minimum marks
- Attendance percentage
- Course availability
- Document verification
### Why Apex?
Complex multi-step logic is easier and more efficient using code.

---
# Pseudocode Examples
## Example 1: Course Seat Validation
IF course seats are full
THEN block student registration
ELSE allow admission
## Example 2: Attendance Notification
IF attendance percentage < 75%
THEN send warning notification to student
Example 3: Scholarship Eligibility
IF marks > 90%
AND attendance > 85%
THEN approve scholarship
ELSE reject scholarship request
Why Enterprise Systems Need Programming
Enterprise systems handle:
Large amounts of data
Complex workflows
Advanced business rules
External integrations
No-code tools are powerful but have limitations. Programming provides flexibility and allows businesses to implement custom solutions efficiently.

### Reflection
Not all enterprise logic can be built using only clicks and configuration because businesses often require:
Complex calculations
Dynamic conditions
External system integrations
High-performance automation
Apex helps developers build scalable and flexible enterprise applications beyond the limits of declarative tools.

### Reflective Questions
1. Why is Apex needed if Salesforce already has Flows?
Apex is needed for advanced business logic, integrations, and complex automation that Flows cannot efficiently handle.

2. When should developers prefer no-code solutions?
Developers should prefer no-code solutions when requirements are simple, easy to maintain, and do not require advanced logic.

3. What problems require custom programming?
Complex calculations, integrations, advanced validations, and high-level automation require custom programming.

4. Why is business logic important in enterprise systems?
Business logic ensures processes follow company rules and operate correctly.

5. Why should developers avoid unnecessary coding?
Unnecessary coding increases complexity, maintenance effort, and development time.

6. How does programming increase flexibility?
Programming allows developers to create customized solutions based on specific business requirements.

### Trailhead Modules Completed
Apex & .NET Basics
Apex Basics & Database

### Screenshots
(Add Trailhead completion screenshots here)

Conclusion
Day 5 helped in understanding how programming fits into Salesforce development. It explained why Apex is important for implementing advanced business logic and how all Salesforce concepts learned so far work together in a real enterprise application.
