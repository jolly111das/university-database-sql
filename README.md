# University Database (MySQL)

Designed a small relational database for a university, with departments, students and courses. Then wrote SQL queries to answer 10 questions about it.

## Tools
MySQL · SQL (DDL, primary/foreign keys, JOINs, LEFT JOIN, GROUP BY, HAVING, LIKE)

## Database design
| Table | Columns |
|---|---|
| `Departments` | DepartmentID (PK), DepartmentName |
| `Students` | StudentID (PK), Name, Age, DepartmentID (FK → Departments) |
| `Courses` | CourseID (PK), CourseName, StudentID (FK → Students) |

The database has 3 departments, 5 students and 10 course enrolments.

## Questions answered
1. All student details with their department names
2. Students enrolled in *Artificial Intelligence*
3. Number of students in each department
4. Courses taken by *Alice Johnson*
5. Students enrolled in more than one course (`HAVING`)
6. Average student age per department
7. Department with the most students
8. Students **not** enrolled in any course (`LEFT JOIN ... IS NULL`)
9. Total number of courses for each student
10. Computer Science students taking a course with "Data" in its name (`LIKE`)

The output of each query is saved in the `screenshots/` folder (`Q1.png` to `Q10.png`).

## Files
| File | Description |
|---|---|
| `universityDB.sql` | Table creation, sample data and all 10 queries |
| `screenshots/` | Query results from MySQL Workbench |

---
*Assignment completed as part of the Data Analytics program at Topmentor (2026).*
