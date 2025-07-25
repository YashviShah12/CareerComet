# CareerComet - Core Project Concepts

## 🔹 Objects
- **User** (Job Seeker, Employer – from account.models.py)
- **Job**  (– from jobapp.models.py)
- **Application**  (– from jobapp.models.py)
- **Resume**    (– uploaded media files)
- **Subscription**, **Role**   (– role-based access components)
- **Feedback**   (– if implemented)
- **JobController**, **LoginController**   (– logical controllers in views)
- **Admin**   (– superuser/admin actions)
- **Form** (Registration, Login, Job Posting)

## 🔹 Contexts
- User Registration/Login (`account` module)
- Job Posting (`jobapp` module)
- Job Application (`jobapp` module)
- Admin Panel (`admin.py`)
- Subscription Handling (`template/account`)
- Media Management (`media/resumes`)
- Templates Rendering (`template/jobapp`, `template/account`)
- Permissions and Roles (`jobapp/permission.py`)

## 🔹 Important Information per Context

| Context             | Important Information                                                                 |
|---------------------|----------------------------------------------------------------------------------------|
| Registration        | Username, Email, Password, Role (Employer or Jobseeker)                               |

| Job Posting         | Title, Description, Salary, Category, Company, Expiry Date                            |

| Job Application     | Applicant Info, Resume, Job ID, Application Status, Date                              |

| Login               | Credentials, Role Validation                                                           |

| Admin Management    | View/Delete Users, View Feedback, View System Stats                                   |

| Resume Upload       | File type, Path, Link to JobSeeker                                                     |

| Templates           | Forms, Display Logic, Context Variables, Base Inheritance                             |
