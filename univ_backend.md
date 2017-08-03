You're building a backend for a university that requires students to be able to login. Once logged in, the students can view the exam grades for their classes. They should be able to view results by semester. Each semester should only show the classes in which that student is enrolled that semester.

# Needs
* Students
  * logged in?
  * semester
    * courses
      * grades

## Model

```javascript
  student: {
    logged: Boolean,
    semesters: [
      semester: {
        courses: [
          course: {
            name: String,
            id: Number,
            grade: Number,
            feedback: String,
            reprimands: Number,
            rateMyProfLink: String
          }
        ]
      }
    ]
  }

```
