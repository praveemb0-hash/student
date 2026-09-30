# Student Enrollment & Course Management System (SECMS)

A Salesforce DX implementation of a Student Enrollment & Course Management System. The repository models Students, Courses, Instructors and Enrollments and provides validation, automation, approval, reporting, dashboard and security metadata.

## Features
- Student, Course, Instructor and Enrollment custom objects
- Lookup relationships from Enrollment to Student, Course and Instructor
- New Enrollment and Re-Enrollment record types
- Institutional email validation
- Fee-before-approval validation
- Enrollment-date automation
- Instructor assignment by course category
- Follow-up task automation for requested enrollments
- Approval-process metadata/documented setup
- Reports and Student Management dashboard metadata
- Admin, Enrollment Officer and Instructor permission sets
- Fictional sample CSV data

## Architecture
Salesforce Lightning UI -> Custom Objects -> Validation Rules / Flow Automation -> Approval -> Reports & Dashboard -> Security controls.

## Prerequisites
- Salesforce Developer Org
- Salesforce CLI (`sf`)
- VS Code with Salesforce Extension Pack

## Quick start
```bash
sf org login web --alias secms-dev
sf project deploy start --source-dir force-app --target-org secms-dev
sf org open --target-org secms-dev
```

Load sample data after deployment using Data Import Wizard or `sf data import tree` as appropriate. Because lookup IDs are org-specific, the included CSVs are intentionally seed data rather than hard-coded Salesforce record IDs.

## Main objects
| Object | API Name | Purpose |
|---|---|---|
| Student | Student__c | Student profile and status |
| Course | Course__c | Course catalogue and fees |
| Instructor | Instructor__c | Instructor expertise/contact |
| Enrollment | Enrollment__c | Student course enrollment lifecycle |

## Automation
See `docs/AUTOMATION.md` for the four requested flows and their expected behavior.

## Security
Permission sets are provided as a portable baseline. Organization-wide sharing and user-specific approver/owner configuration may require Setup in the target org; see `docs/SECURITY.md`.

## Testing
See `docs/TESTING.md`. Actual deployment/runtime testing must be performed in a Salesforce Developer Org; this repository does not claim that an external org has been deployed or tested.

## Screenshots
No screenshots are fabricated. Follow `docs/SCREENSHOT_GUIDE.md` and add real Salesforce screenshots after deployment.

## GitHub
The repository is designed to be committed directly to GitHub. See `GITHUB_UPLOAD_GUIDE.md`.
