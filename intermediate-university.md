## University Backend

You're building a backend for a university that requires students to be able to login. Once logged in, the students can view the exam grades for their classes. They should be able to view results by semester. Each semester should only show the classes in which that student is enrolled that semester.

Student Document
Classes Document
Semesters?

Student Document:
* username: string
    * Must contain only word characters
* password: string
    * Must be at least 8 characters
* email: string
    * Must contain an @ symbol
* grades: subdocument

Grades Subdocument:
* classname / grade: strings
    * Classname must be key for grade value
    * Classname must be at least 8 characters
    * Grade is MAX 3 characters
* semesters: subdocument

Semesters Subdocument:
* semesterName: {
  "classname": grade
      * Same requirements as above in Grades subdocument
}