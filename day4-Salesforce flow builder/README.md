# Day 4 - Salesforce Flow Builder

# What is Flow Builder?
Flow Builder is a no-code automation tool in Salesforce used to automate business processes using a visual interface.
It helps organizations:
- Reduce manual work
- Improve productivity
- Maintain consistency
- Automate repetitive tasks
- Update records automatically
Flow Builder allows admins and developers to create workflows without writing code.

---
# Why Automation Matters
Businesses perform many repetitive tasks daily. Manual handling of these tasks can cause:
- Human errors
- Delays
- Data inconsistency
- Increased workload
Automation helps by:
- Saving time
- Improving accuracy
- Increasing efficiency
- Reducing repetitive work

---
# Types of Flows in Salesforce

## 1. Screen Flow
Screen Flow is an interactive flow where users provide input through screens.
### Features:
- User interaction
- Forms and input fields
- Guided business processes
### Example:
Student registration form.

---
## 2. Record-Triggered Flow
Record-Triggered Flow runs automatically when a record is created, updated, or deleted.
### Features:
- Fully automated
- Runs in background
- No user interaction required
### Example:
Automatically sending an email when a student registers.

---
# Difference Between Screen Flow and Record-Triggered Flow

| Screen Flow                    | Record-Triggered Flow            |
|--------------------------------|----------------------------------|
| Requires user interaction      | Runs automatically               |
| Contains screens/forms         | Background automation            |
| Used for guided processes      | Used for automatic updates       |
| Example: Admission form        | Example: Auto email notification |

---

# Automation Ideas for College Management System
## 1. Auto Email After Registration
### Process:
Send confirmation email automatically after student registration.
### Why Automation Helps:
Reduces manual communication and improves student experience.

---
## 2. Auto Update Remaining Seats
### Process:
Automatically reduce available seats when a student enrolls.
### Why Automation Helps:
Maintains accurate seat availability without manual updates.

---
## 3. Notify Faculty When Course Is Full
### Process:
Send notification to faculty when enrollment reaches maximum capacity.
### Why Automation Helps:
Helps faculty manage admissions efficiently.

---
## 4. Generate Student ID Automatically
### Process:
Automatically generate a unique student ID after admission.
### Why Automation Helps:
Avoids duplicate IDs and reduces manual work.

---
## 5. Send Fee Deadline Reminder
### Process:
Automatically send reminders before fee payment deadline.
### Why Automation Helps:
Improves fee collection and reduces missed payments.

---

# Flow Design Thinking

## Selected Automation:
Auto Email After Student Registration

---

# Flow Diagram

```text
Student Record Created

          │
          ▼
Check Student Email Exists?
          │
     ┌────┴────┐
     │         │
    Yes        No
     │         │
     ▼         ▼
Send Email   Stop Flow
     │
     ▼
Update Status
     │
     ▼
Flow Ends
