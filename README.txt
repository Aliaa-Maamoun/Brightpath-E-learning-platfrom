# E-Learning Platform

This is a **simple E-Learning Platform** implemented with **HTML, CSS, JavaScript (using Bootstrap)** for the frontend and **PHP** for the backend.

---

## 🔹 Project Contents

- **SRS File:** Detailed Software Requirements Specification
- **Jira Report:** Report of issues, progress, and timelines
- **UML Diagrams:** Class, Use Case, and Architectural Diagrams
- **PowerPoint Presentation:** Summary and walkthrough of the project

---

## 🔹 Tech Stack

- **Frontend:** HTML, CSS, JavaScript, Bootstrap
- **Backend:** PHP
- **Database:** MySQL
- **Server:** Apache (using WAMP or XAMPP)

---

## 🔹 Installation and Setup

### 1️⃣ Install WAMP or XAMPP
- Download and install [XAMPP](https://www.apachefriends.org/) or [WAMP](https://www.wampserver.com/) on your computer.

### 2️⃣ Run Apache and MySQL
- Start Apache and MySQL services from the control panel.

### 3️⃣ Set up Database:

➥ Open your browser and navigate to: your"http://localhost/phpmyadmin/"
➥ Username: `root`
➥ Password: (leave it empty)

➥ Once phpMyAdmin opens:
- Select **Databases**
- Name your database: `loginsystemtut`
- Then click **Create**

---

### 4️⃣ Create `users` table:

➥ Select `loginsystemtut`
➥ Open the **SQL** tab
➥ Execute:

```sql
CREATE TABLE users (
	idUsers int(11) AUTO_INCREMENT PRIMARY KEY NOT NULL,
	uidUsers TINYTEXT NOT NULL,
	emailUsers TINYTEXT NOT NULL,
	pwdUsers LONGTEXT NOT NULL
);
## 5️⃣ Create `imgupload` table:

➥ Still under `loginsystemtut`.  
➥ Open **SQL tab** again and execute:

```sql
CREATE TABLE imgupload (
	id int(11) NOT NULL AUTO_INCREMENT PRIMARY KEY,
	userid int(11) NOT NULL,
	status int(11) NOT NULL
);
```

## 6️⃣ Deployment:

➥ Move or copy the folder `e-learning` into:

```bash
xampp/htdocs/
```

or

```bash
wamp/www/
```

➥ Access the application by navigating to:

```arduino
http://localhost/e-learning/
```

## 🔹 File overview 

```pgsql
e-learning/
├── docs/
│ ├─ SRS.pdf
│ ├─ Jira_report.pdf
│ ├─ Class_diagram.png
│ ├─ Use_case_diagram.png
│ └─ Project_presentation.pptx
├── css/
├── imgs/
├── js/
├── index.php
├── login.php
├── register.php
├── README.md
```

## 🔹 Notes

➥ The **SRS**, **Jira Report**, **UML Diagrams**, and **PowerPoint Presentation** files are located in the `docs/` directory.  
➥ The application lets you:
- Register and login.
- Handle photo/image upload.

## 🔹 Contributors

Developer: [Your Name]  
Design: [Your Name]  
Tester: [Your Name]  

## 🔹 License

This project is for educational purposes and is licensed under the MIT License.
