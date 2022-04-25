# database

## Triggers

- increase_class_size: When a student enroll a class, then update the class size
- decrease_class_size: When a student drop a class, then update the class size
- increase_class_total_attendance_times: When a roll call start, then update the total attendance times of the class
- update_attendance_record: When a roll call start, then put all the students(no professor) with uncheck status into the attendance record
- update_attendance_rate_when_updated: When a record changed, then update the attendance rate of the roll call and student, the records are not allowed to change after the expired time
- update_attendance_rate_when_inserted: When a roll call started, then update the attendance rate of the student, the records are not allowed to change after the expired time
- delete_roll_call: delete the related record when delete a roll call
- delete_class: delete the related rows in class_enrolled table, roll_coll table, attendance_record table

## Structure

<img width="712" alt="structure" src="https://user-images.githubusercontent.com/38137877/165018846-832c421c-f28c-47ab-babf-b5617de858fe.png">

