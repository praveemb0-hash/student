# Automation

## SetEnrollmentDate
Trigger: Enrollment creation. Expected result: Enrollment Date is set to the current date.

## Enrollment_Approved_Action
Trigger: Enrollment becomes Approved. Expected result: related Student becomes Active and notification actions are performed where configured.

## AutoAssign_Instructor
Trigger: Enrollment created/updated. Expected result: Technical -> INSTR_A, Language -> INSTR_B, Non-Technical -> INSTR_C.

## Create_Followup_Task
Trigger: Enrollment Status = Requested. Expected result: a follow-up Task is created for the appropriate administrator with due date two days later.

The repository includes named Flow metadata shells as a safe source baseline. Review and complete runtime actions/activation in Flow Builder for the target org before production use.
