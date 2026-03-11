# MAD-1-Placement-Portal-Application-
The Placement Portal Application is a centralized platform that automates campus recruitment by replacing manual spreadsheets and emails. It streamlines company registrations, tracks student applications in real-time, and ensures accurate placement records through a unified interface for administrators, recruiters, and students.

# Placement Portal Application

## Project Overview

The **Placement Portal Application** is a web-based system developed to streamline campus recruitment activities within educational institutions. It provides a centralized platform where **Admin (Institute Placement Cell), Companies, and Students** can interact efficiently to manage placement drives, applications, and recruitment processes.

The application eliminates the need for manual processes such as spreadsheets and emails by automating company approvals, placement drive creation, and student application tracking.

This system ensures better management of recruitment activities and maintains structured records for all placement-related operations.

---

# Problem Statement

Many educational institutions manage campus recruitment activities manually using spreadsheets and emails. This approach often leads to:

* Difficulty managing company registrations
* Inefficient tracking of placement drives
* Duplicate student applications
* Lack of centralized application records
* Poor tracking of placement status

The Placement Portal Application addresses these issues by providing an automated and role-based platform for managing recruitment workflows.

---

# System Roles

## Admin (Institute Placement Cell)

The Admin acts as the system supervisor and has complete control over the platform.

Admin functionalities include:

* Approve or reject company registrations
* Approve or reject placement drives created by companies
* View and manage students, companies, and placement drives
* Search students by name, ID, or contact information
* Search companies by name
* Blacklist or deactivate accounts
* View all job applications and placement history

---

## Company

Companies register on the portal and conduct placement drives for recruitment.

Company functionalities include:

* Create and manage company profile
* Create placement drives/job postings
* Edit or close job postings
* View student applications
* Shortlist or reject candidates
* Update application status (Shortlisted / Selected / Rejected)
* View student profiles and resumes

---

## Student

Students can participate in campus recruitment through the portal.

Student functionalities include:

* Register and log in
* Update profile details
* Upload resume
* View approved placement drives
* Apply for placement drives
* Track application status
* View placement history

---

# Key Features

* Role-based authentication (Admin, Company, Student)
* Company approval workflow
* Placement drive creation and management
* Student application tracking
* Resume upload functionality
* Prevention of duplicate job applications
* Admin dashboard with system statistics
* Application status updates
* Complete application history tracking

---

# Technology Stack

| Component       | Technology                  |
| --------------- | --------------------------- |
| Backend         | Flask (Python)              |
| Frontend        | HTML, CSS, Bootstrap        |
| Template Engine | Jinja2                      |
| Database        | SQLite                      |
| Authentication  | Flask Session / Flask-Login |
| API Definition  | OpenAPI YAML                |

---

# Project Structure

```
placement_portal/

app.py
config.py
models.py

routes/
   auth_routes.py
   admin_routes.py
   company_routes.py
   student_routes.py

templates/
   admin/
   company/
   student/
   auth/

static/
   css/
   uploads/

instance/
   placement_portal.db

README.md
requirements.txt
api.yaml
```

---

# Database Entities

The system uses the following main tables:

* Admin
* Company
* Student
* PlacementDrive
* Application

Relationships:

Company → PlacementDrive
Student → Application
PlacementDrive → Application

---

# Installation and Setup

## 1. Clone the Repository

```bash
git clone https://github.com/your-repository-link
cd placement-portal
```

## 2. Install Dependencies

```bash
pip install -r requirements.txt
```

## 3. Run the Application

```bash
python app.py
```

## 4. Open in Browser

```
http://127.0.0.1:5000
```

---

# Default Admin Login

Admin account is predefined in the system.

Example credentials:

Username: admin
Password: admin123

---

# API Documentation

The API specification file is included as:

```
api.yaml
```

It defines endpoints related to:

* Student data
* Placement drives
* Applications

---

# Demo Video

Project demonstration video:

```
Add your Google Drive video link here
```

Ensure the link is accessible to **Anyone with the link**.

---

# AI / LLM Usage Declaration

AI tools such as ChatGPT were used only for documentation formatting, guidance, and improving code readability.
Approximate usage: **10–15%**
All major development, debugging, and integration were performed manually.

---

# Future Enhancements

* Email notifications for application updates
* Interview scheduling system
* Advanced analytics dashboard
* Resume screening automation
* Integration with external job portals

---

# Author
Harshad Bharat Gangurde
23f2004217@ds.study.iitm.ac.in
IIT Madras BS Degree Program
