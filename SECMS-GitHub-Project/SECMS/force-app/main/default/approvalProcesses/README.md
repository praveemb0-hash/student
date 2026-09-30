# Approval Process

The SECMS specification requires an approval process named `Approval_Enrollment_Request` on `Enrollment__c` with entry criteria `Enrollment_Status__c = Requested`, Training Manager approval, final approval status `Approved`, and final rejection status `Rejected`.

Salesforce approval-process metadata is org/user dependent in several areas. Configure the approver/user and activate the process in Setup after deploying the portable object, field, validation, flow, app, report, dashboard and permission metadata.
