# Object Model

```text
Student (1) --------< Enrollment >-------- (1) Course
                          |
                          |
                          v
                     Instructor (1)
```

## Student__c
Student Name, Email, Phone, Date of Birth, Student Status, Address.

## Course__c
Course Name, Category, Duration, Course Fee, Description.

## Instructor__c
Instructor Name, Instructor Code, Expertise, Phone, Email.

## Enrollment__c
Enrollment Name, Student, Course, Instructor, Enrollment Date, Enrollment Status, Fees Paid, Total Amount, Comments.
