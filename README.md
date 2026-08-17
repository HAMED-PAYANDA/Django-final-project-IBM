<div align="center">

# 🌐 Full-Stack Django Web Application

A comprehensive full-stack web application built using the Django framework, demonstrating backend server logic, dynamic frontend rendering, and relational database management.

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Django](https://img.shields.io/badge/Django-Web_Framework-092E20?style=for-the-badge&logo=django&logoColor=white)](https://www.djangoproject.com/)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-Frontend-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)](https://getbootstrap.com/)
[![IBM Certification](https://img.shields.io/badge/IBM-Full%20Stack%20Software%20Developer%20Professional-blue?style=for-the-badge&logo=ibm)](https://www.coursera.org/professional-certificates/ibm-full-stack-cloud-developer)
[![IBM](https://img.shields.io/badge/IBM-Capstone_Project-052FAD?style=for-the-badge&logo=ibm&logoColor=white)](#)
[![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)](#)

</div>

---

## 📌 Project Overview

This repository serves as the capstone project for the **IBM Full-Stack Software Developer** curriculum. It demonstrates the end-to-end development of a database-driven web application using **Django**. 

The project showcases the ability to handle user authentication, manage relational data using Django Models, route HTTP requests, and render dynamic content seamlessly using Django Templates and Bootstrap.

---

## 🏗️ Architecture: Model-View-Template (MVT)

This application strictly adheres to Django's standard MVT design pattern to ensure a clean separation of concerns between the database layer, the business logic, and the user interface.

```text
┌─────────────────┐       ┌─────────────────┐       ┌─────────────────┐
│                 │ Request                 │       │                 │
│ Browser / Client│ ──────> URL Dispatcher  │ ──────>   Django View   │
│                 │ <──────                 │ <──────                 │
└─────────────────┘ Response└─────────────────┘       └──────┬───┬──────┘
                                                             │   │
                                          Database Read/Write│   │Context Data
                                                             ▼   ▼
                                        ┌─────────────────┐ ┌───────────────┐
                                        │  Django Models  │ │Django Template│
                                        │ (SQLite/DB logic) │ (HTML / CSS)  │
                                        └─────────────────┘ └───────────────┘
```
✨ Key Features Implemented
•	User Authentication: Secure user registration, login, and logout functionality.
•	Database Management: Custom Django Models mapping to a relational database to store users, entities, and reviews.
•	Django Admin Integration: A fully configured superuser dashboard to easily manage database entries via a graphical interface.
•	Dynamic Frontend: HTML templates infused with Django Template Language (DTL) tags to render server-side data directly to the user.
•	Responsive UI: Integration with Bootstrap to ensure the application is mobile-friendly and highly accessible.

🛠️ Core Tech Stack
## 🛠️ Core Tech Stack

| Category | Technologies Used | Purpose |
| :--- | :--- | :--- |
| **Backend Framework**| Python, Django | Core server logic, routing, and HTTP request handling |
| **Frontend UI** | HTML5, CSS3, Bootstrap | Structuring and styling the user-facing web pages |
| **Database** | SQLite / ORM | Relational data storage managed via Django's ORM |
| **Version Control** | Git, GitHub | Codebase management and continuous tracking |

## ⚙️ Local Setup & Execution

# Django Cloud App with Database
Overview
This is a Django-based web application that allows users to explore courses, enroll, take exams, and view results. The app includes user authentication, instructor and learner roles, and dynamic course content management.
The project was developed as part of a full-stack web development course, focusing on cloud-ready applications with database integration.
Features
User Authentication: Registration, login, logout.
Course Management: View courses, lessons, and associated content.
Enrollment: Learners can enroll in courses and track progress.
Exams:
Multiple-choice questions with multiple correct answers
Submissions tracked per learner
Real-time grading and feedback
Color-coded exam result display (correct, wrong, not selected)
Instructor Role: Ability to manage courses and lessons.
Responsive UI: Built with Bootstrap 4.5 for mobile and desktop friendliness.
Technologies Used
Backend: Django 3.x
Frontend: HTML, Bootstrap 4.5, JavaScript, jQuery
Database: SQLite (default for Django)
Version Control: Git, GitHub

**General Notes**

An `onlinecourse` app has already been provided in this repo upon which you will be adding a new assesement feature.

- If you want to develop the final project on Theia hosted by [IBM Developer Skills Network](https://labs.cognitiveclass.ai/), you will need to create the same project structure on Theia workspace and save it everytime you close the browser
- Or you could develop the final project locally by setting up your own Python runtime and IDE
- Hints for the final project are left on source code files
- You may choose any cloud platform for deployment (default is IBM Cloud Foundry)
- Depends on your deployment, you may choose any SQL database Django supported such as SQLite3, PostgreSQL, and MySQL (default is SQLite3)

**ER Diagram**
For your reference, we have prepared the ER diagram design for the new assesement feature.

![Onlinecourse ER Diagram](https://github.com/ibm-developer-skills-network/final-cloud-app-with-database/blob/master/static/media/course_images/onlinecourse_app_er.png)
=======
⚙️ Local Setup & Execution
To run this Django application on your local machine, follow these steps:
1. Clone the Repository
```text
git clone [https://github.com/HAMED-PAYANDA/Django-final-project-IBM.git](https://github.com/HAMED-PAYANDA/Django-final-project-IBM.git)
cd Django-final-project-IBM
```

2. Install Dependencies
```text
Ensure you have Python installed, then install the required Django packages:
python3 -m pip install -r requirements.txt
```

3. Apply Database Migrations
Prepare the SQLite database by applying the built-in and custom Django migrations:
```text
python3 manage.py makemigrations
python3 manage.py migrate
```

4. Create a Superuser (Optional but Recommended)
To access the Django Admin dashboard (/admin), create an administrative account:
```text
python3 manage.py createsuperuser
```

5. Run the Development Server
Launch the application locally:
```text
python3 manage.py runserver
```

The application will now be accessible in your web browser at http://127.0.0.1:8000/.

---

## License
This project is licensed under the [Apache 2.0 License](LICENSE).

## 👤 Author

**Hamed Payanda**
* **GitHub:** [@HAMED-PAYANDA](https://github.com/HAMED-PAYANDA)
* Completed as part of the **IBM Full-Stack Software Developer Professional**.



