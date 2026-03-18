<h1>Course Withdrawal Application</h1>
 
<p>A desktop-based application that allows students to formally request course withdrawals and enables administrators to review and process those requests.</p>

---
 
## Technologies Used
 
| Technology | Purpose |
|---|---|
| Java | Core programming language |
| Java Swing / AWT | Graphical User Interface (GUI) |
| MySQL | Database |
| JDBC | Database connectivity |
| NetBeans IDE | Development environment |
 
---
 
## Project Overview
 
The **Course Withdrawal Application** is an online system that enables:
 
- **Students** to submit withdrawal requests, track their status, and view policies
- **Admins** to review, approve, or reject withdrawal requests and manage policies
 
---
 
## Features
 
### For Students
- View enrolled and unenrolled courses
- Submit a course withdrawal request
- Track status of submitted requests (Pending / Approved / Rejected)
- View withdrawal policies
- View withdrawal deadline
 
### For Administrators
- View students semester-wise and their enrollments
- Review and process withdrawal requests
- Edit withdrawal policies
- Edit withdrawal deadline
 
---
 
## Database
 
- **Database Name:** `studentsdata`
- **Tables:** `students`, `semesters`, `courses`, `enrollments`, `withdrawalrequests`, `policies`
 
> See `sql_tables.txt` for all SQL CREATE TABLE statements.
 
---
 
## Setup & Installation
 
> See `instructions.txt` for complete step-by-step setup guide.
 
---
 
## Login Credentials
 
| Role | ID | Password |
|---|---|---|
| Student | (from students table) | (set during data insertion) |
| Admin | `Admin` | `123` |
 
---
 
## Data Structures Used
 
| Structure | Location | Purpose |
|---|---|---|
| `Stack<JFrame>` | `WithdrawApplication.java` | Tracks visited frames for Back button |
| `LinkedList<Course>` | `Student.java` | Stores student's enrolled courses |
| `ArrayList<Queue<Request>>` | `WithdrawApplication.java` | Stores requests per semester (8 queues) |
 
---
 
## 📁 Project Structure
 
```
CourseWithdrawalApp/
├── src/
│   ├── WithdrawApplication.java    # Main class + data structures
│   ├── Student.java                # Student model
│   ├── Course.java                 # Course model
│   ├── Request.java                # Request model
│   ├── LoginPage.java              # Login frame
│   ├── StudentDashboard.java       # Student dashboard
│   ├── AdminDashboard.java         # Admin dashboard
│   ├── EnrolledCourses.java        # View enrolled courses
│   ├── UnenrolledCourses.java      # View withdrawn courses
│   ├── WithdrawCourse.java         # Withdrawal form
│   ├── TrackApplications.java      # Track requests
│   ├── ViewPolicies.java           # View policies
│   └── ViewDeadline.java           # View deadline
├── README.md
├── instructions.txt
└── sql_tables.txt
```
For clone use this link : https://github.com/RadhikaKapoor383/Course-Withdrawal-App.git
 
---
 
## Additional Files
 
- `instructions.txt` — Full setup and usage guide
- `sql_tables.txt` — All SQL CREATE TABLE and INSERT statements
