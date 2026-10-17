# Vacation Tracking System (VTS) — Requirements Analysis

## 1. Vision

To enable employees to manage their own vacation time, sick leave, and personal time off without requiring expert knowledge of company or local leave policies, through an easy-to-use and intuitive system.

The system aims to automate vacation management, reduce manual HR processing, minimize the time required to handle vacation requests, and allow employees to manage their leave more independently.

## 2. Functional Requirements (FR)

1- The system shall allow employees to create new vacation requests.

2- The system shall allow employees to edit pending vacation requests.

3- The system shall allow employees to withdraw requests that are pending approval.

4- The system shall allow employees to cancel approved vacation requests according to the applicable cancellation rules.

5- The system shall validate vacation requests against applicable company and location-specific leave policies and display errors when the submitted data is incomplete or invalid.

6- The system shall allow managers to approve or reject vacation requests submitted by their subordinates. A rejection shall require an explanation.

7- The system shall send an email notification to the authorized manager when a valid vacation request requires approval.

8- The system shall update the vacation request status to approved or rejected based on the manager's decision.

9- The system shall send an email notification to the employee when the manager approves or rejects a vacation request.

10- The system shall update the request status to withdrawn when an employee confirms the withdrawal of a pending request and notify the manager.

11- The system shall return the applicable vacation time allowance to the employee when an approved vacation request is successfully canceled.

## 3. Non-Functional Requirements (NFR)

### (Usability)

1- The Vacation Tracking System shall be easy to use and intuitive, allowing employees to manage their vacation requests without requiring expert knowledge of company or local leave policies.

### (Security)

**1- Authentication:**

a- The system shall authenticate users through the existing intranet portal's Single Sign-On (SSO) mechanism.

**2- Authorization:**

a- The system shall restrict access to functions and employee information based on the authenticated user's assigned role and privileges.

### (Auditability / Traceability)

1- The system shall maintain activity logs for all transactions to support auditing and traceability.

2- The system shall log administrative overrides of actions restricted by the applicable rules.

## 4. Constraints

1- The Vacation Tracking System must use the organization's existing hardware and middleware.

2- The system must be implemented as an extension to the existing company intranet portal.

3- The system must use the existing intranet portal's Single Sign-On (SSO) mechanism for authentication.

4- The system must integrate with the existing HR legacy systems to retrieve employee information and updates.


5- All employees work eight-hour days.

6- Vacation request validation rules are defined and owned by the HR department.

7- Manager approval is required only when applicable under the system's rules.

## 5. Actors

**1- Employee**

 Employees can manage their own vacation time, including submitting, viewing, editing, withdrawing, and canceling vacation requests according to the applicable rules.

**2- Manager**

A specialized employee role with additional responsibilities for approving or rejecting vacation requests submitted by subordinates and awarding additional leave time within system-defined limits.

**3- HR Clerk**

Responsible for maintaining employee information, leave categories, location records, and applicable vacation policies.

**4- System Admin**

Responsible for maintaining the system's technical resources, collecting and archiving system logs, and supporting system administration.