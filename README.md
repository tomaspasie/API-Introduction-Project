# API Introduction Project

### Goal: Document REST API using the Swagger Editor to generate API Documentation and the finished code into a YML file.

# School REST API Documentation  

## User Management  

```
/user_management:
    get:
      tags:
      - user_management
      summary: Get Users
      description: Browse All Users OR Retrieve One User
      operationId: getUser
      parameters:
      - name: User
        in: query
        description: A member of the school.
        schema:
          type: string
      responses:
        400:
          description: Invalid user
          content: {}
  /user_management/:
    put:
      tags:
      - user_management
      summary: Edit User
      description: Edit One User
      operationId: putUser
      parameters:
      - name: User
        in: query
        description: A member of the school.
        schema:
          type: string
      responses:
        400:
          description: Invalid user
          content: {}
  /user_management/delete:
    delete:
      tags:
      - user_management
      summary: Delete User
      description: Delete One User
      operationId: deleteUser
      parameters:
      - name: User
        in: query
        description: A member of the school.
        schema:
          type: string
      responses:
        400:
          description: Invalid user
          content: {}
```

#### BREAD Queries
- GET: All Users (Browse) OR One User (Retrieve)
- PUT: One User (Edit)
- DELETE: One User (Delete)

## Course Management  

```
  /course_management:
    get:
      tags:
      - course_management
      summary: Get Courses
      description: Browse All Courses OR Retrieve One Course
      operationId: getCourse
      parameters:
      - name: Course
        in: query
        description: A course a student takes.
        schema:
          type: string
      responses:
        400:
          description: Invalid course
          content: {}
  /course_management/:
    put:
      tags:
      - course_management
      summary: Edit Course
      description: Edit One Course
      operationId: putCourse
      parameters:
      - name: Course
        in: query
        description: A course a student takes.
        schema:
          type: string
      responses:
        400:
          description: Invalid course
          content: {}
  /course_management/delete:
    delete:
      tags:
      - course_management
      summary: Delete Course
      description: Delete One Course
      operationId: deleteCourse
      parameters:
      - name: Course
        in: query
        description: A course a student takes.
        schema:
          type: string
      responses:
        400:
          description: Invalid course
          content: {}
```

#### BREAD Queries
- GET: All Courses (Browse) OR One Course (Retrieve)
- PUT: One Course (Edit)
- DELETE: One Course (Delete)

## Course Assignment Management  

```       
  /course_assignment_management:
    get:
      tags:
      - course_assignment_management
      summary: Get Assignments
      description: Browse All Assignments OR Retrieve One Assignment
      operationId: getAssignment
      parameters:
      - name: Assignment
        in: query
        description: An assignment to be added to courses.
        schema:
          type: string
      responses:
        400:
          description: Invalid assignment
          content: {}
  /course_assignment_management/:
    put:
      tags:
      - course_assignment_management
      summary: Edit Assignment
      description: Edit One Assignment
      operationId: putAssignment
      parameters:
      - name: Assignment
        in: query
        description: An assignment to be added to courses.
        schema:
          type: string
      responses:
        400:
          description: Invalid assignment
          content: {}
  /course_assignment_management/delete:
    delete:
      tags:
      - course_assignment_management
      summary: Delete Assignment
      description: Delete One Assignment
      operationId: deleteAssignment
      parameters:
      - name: Assignment
        in: query
        description: An assignment to be added to courses.
        schema:
          type: string
      responses:
        400:
          description: Invalid assignment
          content: {}
```

#### BREAD Queries
- GET: All Assignments (Browse) OR One Assignment (Retrieve)
- PUT: One Assignment (Edit)
- DELETE: One Assignment (Delete)

## Course Section Management  

```
  /course_section_management/:
    put:
      tags:
      - course_section_management
      summary: Edit Section
      description: Edit One Section
      operationId: putSection
      parameters:
      - name: Section
        in: query
        description: A section to enroll teachers and students in.
        schema:
          type: string
      responses:
        400:
          description: Invalid section
          content: {}
  /course_section_management/delete:
    delete:
      tags:
      - course_section_management
      summary: Delete Section
      description: Delete One Section
      operationId: deleteSection
      parameters:
      - name: Section
        in: query
        description: A section to enroll teachers and students in.
        schema:
          type: string
      responses:
        400:
          description: Invalid section
          content: {}
```

#### BREAD Queries
- GET: All Sections (Browse) OR One Section (Retrieve)
- PUT: One Section (Edit)
- DELETE: One Section (Delete)

## Section Enrollment Management  

```
/section_enrollment_management/:
    put:
      tags:
      - section_enrollment_management
      summary: Edit Section
      description: Edit One Section
      operationId: putSectionEnrollment
      parameters:
      - name: Section
        in: query
        description: A section to assign teachers and students to.
        schema:
          type: string
      responses:
        400:
          description: Invalid section
          content: {}
  /section_enrollment_management/delete:
    delete:
      tags:
      - section_enrollment_management
      summary: Delete Section
      description: Delete One Section
      operationId: deleteSectionEnrollment
      parameters:
      - name: Section
        in: query
        description: A section to assign teachers and students to.
        schema:
          type: string
      responses:
        400:
          description: Invalid section
          content: {}
```

#### BREAD Queries
- GET: All Sections (Browse) OR One Section (Retrieve)
- PUT: One Section (Edit)
- DELETE: One Section (Delete)

## Section Assignment Submission Management  

```
/section_assignment_submission_management:
    get:
      tags:
      - section_assignment_submission_management
      summary: Get Assignment Submissions
      description: Browse All Assignments OR Retrieve One Assignment
      operationId: getAssignmentSubmission
      parameters:
      - name: Assignment
        in: query
        description: An assignment submission.
        schema:
          type: string
      responses:
        400:
          description: Invalid assignment submission
          content: {}
  /section_assignment_submission_management/:
    put:
      tags:
      - section_assignment_submission_management
      summary: Edit Assignment Submission
      description: Edit One Assignment
      operationId: putAssignmentSubmission
      parameters:
      - name: Assignment
        in: query
        description: An assignment submission.
        schema:
          type: string
      responses:
        400:
          description: Invalid assignment submission
          content: {}
  /section_assignment_submission_management/delete:
    delete:
      tags:
      - section_assignment_submission_management
      summary: Delete Assignment Submission
      description: Delete One Assignment Submission
      operationId: deleteAssignmentSubmission
      parameters:
      - name: Assignment
        in: query
        description: An assignment submission.
        schema:
          type: string
      responses:
        400:
          description: Invalid assignment submission
          content: {}
```

#### BREAD Queries
- GET: All Assignments (Browse) OR One Assignment (Retrieve)
- PUT: One Assignment (Edit)
- DELETE: One Assignment (Delete)

