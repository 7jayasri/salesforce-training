# Day 3 - Salesforce Data Modeling

# What is Data Modeling in Salesforce?
Data modeling is the process of organizing and structuring business data in Salesforce using objects, fields, and relationships.
It helps companies:
- Store data efficiently
- Maintain consistency
- Build scalable systems
- Improve reporting and automation

---

# Difference Between App, Object, Record, and Field
| Component | Description                                | Example                |
|-----------|--------------------------------------------|------------------------|
| App       | Collection of related features and objects | College Management App |
| Object    | Database table that stores data            | Student Object         |
| Record    | Single entry inside an object              | One student’s details  |
| Field     | Individual data attribute                  | Student Name           |

---

# Standard vs Custom Objects
## Standard Objects
Standard objects are pre-built objects provided by Salesforce.
### Examples:
- Account
- Contact
- Opportunity
- Lead
These are commonly used CRM objects.
---

## Custom Objects
Custom objects are user-created objects based on business requirements.
### Examples:
- Student
- Faculty
- Course
- Department
Custom objects help organizations build systems specific to their needs.

---
# College Management System Data Model
## App Name
College Management App
# Objects Used
1. Student
2. Faculty
3. Course
4. Department

---

# Relationships Between Objects

| Parent Object | Child Object | Relationship Type   |
|---------------|--------------|---------------------|
| Department    | Faculty      | Lookup Relationship |
| Department    | Course       | Lookup Relationship |
| Course        | Student      | Lookup Relationship |
| Faculty       | Course       | Lookup Relationship |

---

# Relationship Explanation
## Department → Faculty
One department can have many faculty members.
Example:
- CSE Department
- Multiple faculty members belong to it

---
## Department → Course
One department can offer multiple courses.
Example:
- CSE Department offers Java, DBMS, and AI courses.

---
## Course → Student
One course can have many students enrolled.
Example:
- 100 students enrolled in Java Programming.

---
## Faculty → Course
One faculty member can teach multiple courses.
Example:
- A professor teaches Java and DBMS.

---
# College Management Data Flow Diagram
Department
   │
   ├── Faculty
   │
   └── Course
            │
            └── Student
