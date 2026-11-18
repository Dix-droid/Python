# Fictional sample records (NOT loaded automatically)

This folder contains sample `.txt` records to demonstrate the format required for the final project. The student names and email addresses are fictional.

**Your real system starts with zero students.** The active application reads only from `data/`, not from `sample_data/`; the Administrator adds students using the menu. Do not copy these examples into `data/` unless you deliberately want to preload records for a local demonstration.

Files: `example_students.txt`, `example_enrollments.txt`, `example_grades.txt`. The actual `data/subjects.txt` already has four fictional sample subjects. Each line contains one JSON object.

Corresponding records are linked by `student_id`, `subject_code`, and `enrollment_id`. The grades use the demonstration rule: 30% prelim + 30% midterm + 40% final.

These example files do NOT include real student records, password hashes, or account details.
