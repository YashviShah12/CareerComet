
# 📘 CareerComet - Core Concepts Analysis

This document outlines the key **objects**, **contexts**, and **important information** for the CareerComet job portal project.

---

## 🔹 1. Objects

| Object Name        | Description |
|--------------------|-------------|
| **User**           | Represents any platform user (Job Seeker, Employer, Admin). Stored with fields like email, role, password. |
| **JobSeeker**      | A specific user role who can search and apply for jobs. Includes resume, qualifications, experience. |
| **Employer**       | A user role that can post job listings, view applications, and subscribe to plans. |
| **Job**            | Represents a job posting by an employer. Contains title, description, salary, expiry, etc. |
| **Application**    | A job application submitted by a job seeker. Contains status, job reference, and date. |
| **Subscription**   | Details about employer subscription plans (e.g., Basic, Premium) and validity. |
| **Feedback**       | Feedback provided by both job seekers and employers. |
| **Admin**          | Platform administrator who manages users, reviews reports, and moderates content. |
| **Resume**         | A document uploaded by job seekers and stored under media files. |

---

## 🔹 2. Contexts

| Context Module             | Description |
|----------------------------|-------------|
| **User Registration/Login**| Handled via Django auth system; users register as either Job Seeker or Employer. |
| **Job Posting**            | Employers can post job listings using forms and view/manage them via dashboard. |
| **Job Application**        | Job Seekers browse and apply for jobs. Their applications are tracked by status. |
| **Subscription Management**| Employers must subscribe to plans before posting jobs; handled by forms and validations. |
| **Resume Upload**          | Job seekers upload resumes which are linked to their profile and used in applications. |
| **Admin Panel**            | Admin manages users, subscriptions, jobs, and generates reports. |
| **Bookmarking Jobs**       | Job seekers can save/bookmark jobs for future application. |
| **Feedback System**        | Employers and Job Seekers provide feedback about their experience. |
| **Notifications**          | Email or system-based alerts for job application status, new postings, etc. |

---

## 🔹 3. Important Information (Per Context)

| Context                | Important Information |
|------------------------|------------------------|
| **Registration**       | Email must be unique, password must meet strength requirements, role is selected at registration. |
| **Login**              | Users must be verified and activated to login. Separate redirection based on role. |
| **Job Posting**        | Employers must have an active subscription to post. Jobs require a title, description, expiry date, etc. |
| **Job Application**    | Job seekers can only apply if job is active and not expired. Each application has a status field. |
| **Subscription**       | Subscription plan determines job posting limits. Includes fields like plan type, start date, end date, status. |
| **Resume Upload**      | File must be a valid document (PDF, DOCX). Linked to JobSeeker object. |
| **Admin**              | Admin can deactivate users, delete jobs, and view system analytics. Access restricted to superusers. |
| **Bookmarking**        | Job seeker can bookmark multiple jobs. Stored with timestamps for later reference. |
| **Feedback**           | Feedback includes rating (1-5) and optional comments. Stored with user ID and timestamp. |

---

*Generated for Assignment 1: Concepts Identification for CareerComet Project*
