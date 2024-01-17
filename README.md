Project Title: University Management System

1. 

   Department - Student:
o	Relationship Type: One-to-Many
o	Explanation: One department can have many students, but each student is associated with only one department.
•	Department - Professor:
o	Relationship Type: One-to-Many
o	Explanation: One department can have many professors, but each professor is associated with only one department.
•	Professor - Course:
o	Relationship Type: One-to-Many (assuming a professor can teach multiple courses)
o	Explanation: One professor can teach multiple courses, but each course is taught by only one professor.
•	Course - Student:
o	Relationship Type: Many-to-Many (assuming a student can enroll in multiple courses, and a course can have multiple students)
o	Explanation: A course can have multiple students enrolled, and a student can be enrolled in multiple courses. This is typically implemented using a junction table (e.g., Registration table) that stores pairs of CourseID and StudentID.
registration table is between them

•	Student - Grade:
o	Relationship Type: One-to-Many (assuming a student can have multiple grades)
o	Explanation: One student can have multiple grades (for different courses), but each grade is associated with only one student.
•	Course - Grade:
o	Relationship Type: One-to-Many (assuming a course can have multiple grades, one for each student)
o	Explanation: One course can have multiple grades (one for each student who took the course), but each grade is associated with only one course.

2. Database Schema Design:
   - Based on the ERD, design a normalized relational database schema for the university system.
   - Define appropriate data types, primary keys, foreign keys, and any necessary constraints.

3. Table Creation (SQL):
   - Write SQL statements to create the tables in the database according to the schema.
   - Include necessary constraints such as foreign key relationships, unique constraints, etc.

4. Data Population:
   - Insert realistic and diverse data into each table to simulate a functioning university database.
   - Include data that covers various scenarios (e.g., multiple courses per professor, multiple students in a course).

5. Queries and Reports:Create a set of complex SQL queries to retrieve meaningful information from the database, such as:
      - List all students enrolled in a specific department.
      - Display the highest and lowest grades for each course.
      - Find courses with a high registration count.

6. Normalization: ( The process of separating your data into tables and creating primary keys is called normalization.)
   - Ensure that the database is normalized.

7. Indexing and Performance Optimization:
   - Implement appropriate indexing on key columns to optimize query performance.
   - Analyze and explain the impact of indexing on query performance.
8. Security Measures:
   - Incorporate basic security measures into the database design (e.g., user roles, access permissions).

