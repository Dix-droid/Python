# Student Information System — Video Demonstration Guide

This is a guide for **your own recording and publication**. No video or GitHub repository has been uploaded by this project package.

## Suggested recording flow (8–12 minutes, adjust to your instructor's rules)

1. **Introduction:** State the title, purpose and three or more related records (students, subjects, enrollments, grades). Explain that the application is Python 3, terminal-only, and uses `.txt` files.
2. **First-run login:** Demonstrate creating an admin account locally (or use your existing account). Explain that raw passwords are *never saved*. Demonstrate the password stars that appear as you type (without revealing the password), and open a wide terminal to show the centered layout. Log in and show the welcome screen, logged-in role, date/time, four dashboard statistic cards, passing-rate bar and two-column menu.
3. **File operations:** Show that the starting dashboard has **0 students**, then as Administrator use **Students → Add student** to enter a fictional learner. Afterwards log in as Staff to show that they can view/search but cannot create, edit, or delete student profiles. Add a fictional student. Open `data/students.txt` to show a new JSON-line record was *appended*. Search the student by name/ID. Edit the student's program and show that updates persist in the file. Restart the program and confirm it is still there.
4. **Subjects:** Show the course catalog, add a subject, and search by code/title.
5. **Enrollments:** Enroll an Active student in a subject for a term, search for the new enrollment, and demonstrate that attempting a duplicate enrollment is rejected.
6. **Grades:** Use the enrollment ID to save a prelim, midterm and final grade; explain the 30/30/40 weighted calculation and the Pass/Fail cutoff.
7. **Reports:** Display/export the Population Report and the Subject Performance Report; show the student's Report Card. Open a generated `.txt` report in `reports/`.
8. **Themes:** Open the showroom and compare all six themes (Matrix Green, Amber Vintage, Ocean Blue, Midnight Gold, Royal Purple, and Crimson Classic). Show that the colors update immediately and persist in `data/settings.txt`.
9. **Roles and password management:** As Administrator, add a Staff account. Log out, log in as Staff and show the restricted menus. Demonstrate change password from Settings. **Do not say your password aloud or display it**.
10. **Code explanation:** In `database.py`, point out `open(..., 'r')`, `open(..., 'a')` and atomic writes. In `security.py`, point out salt + PBKDF2 password hashing. In `service.py`, show input validation, relationships and grade/report calculations. In `app.py`, show functions, loops, choices and role-based menus.
11. **Conclusion:** Explain the four connected record types, persistence after restart, safe error handling and what you learned. Say which links you will submit.

## Suggested screenshots

Capture these while running **your own copy of the terminal**:

- `01_login.png`: login screen
- `02_dashboard.png`: first administrator dashboard with zero students
- `12_empty_students.png`: zero student records before data entry
- `03_file_operations.png`: add/edit success message
- `04_student_records.png`: table of saved records
- `05_report.png`: summary report
- `06_theme_customization.png`: theme showroom / color selection
- `08_dashboard_midnight_gold.png`: new Midnight Gold dashboard
- `10_dashboard_royal_purple.png`: new Royal Purple dashboard
- `13_staff_view_only.png`: Staff can search and view student records, but cannot add/edit/delete them

## Submission checklist

- [ ] Python source files and `.txt` samples included in your GitHub repository.
- [ ] README explains system name, features, dependencies, installation and operation.
- [ ] GitHub repo contains screenshots but **not your real usernames/password hashes or private student data**.
- [ ] Your video explains the code and demonstrates major operations.
- [ ] Video uploaded to **YouTube** and **Facebook** with instructor-accessible permissions.
- [ ] GitHub repository uploaded, visible to instructor, and collaborator invitation sent to **natzjun2@gmail.com**.
- [ ] Facebook, YouTube and GitHub links submitted in LMS.

## Notes for presenters

The downloaded student, enrollment and grade text files are initially empty. Any fictional student shown in screenshots was added in a temporary demonstration and is not bundled as a stored record. The four sample subjects are fictional. Account creation is intentionally a local first-run step; no public default password or real credential is bundled. The example grading system is for demonstration only and must not be presented as official school policy.
