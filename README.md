<div align="center">

# Placement Management System

### A Java web application for coordinating campus recruitment

**Student records · Company opportunities · Applications · Interviews · Results**

[![Java](https://img.shields.io/badge/Java-17-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)](https://www.oracle.com/java/)
[![Jakarta Servlet](https://img.shields.io/badge/Jakarta%20Servlet-5.0-007396?style=for-the-badge)](https://jakarta.ee/)
[![MySQL](https://img.shields.io/badge/MySQL-8-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.mysql.com/)

[Portfolio](https://rounakshaw2004.github.io/potfolio/) · [LinkedIn](https://linkedin.com/in/rounak-shaw-271a16321) · [GitHub](https://github.com/rounakshaw2004)

</div>

## Project overview

The **Placement Management System** brings core campus recruitment records into one web application. Placement teams can keep student and company information organized, follow applications, schedule interviews, and record final outcomes. The project demonstrates how a Java web stack can connect a browser-based workflow to structured MySQL data.

## Core modules

| Module | What it supports |
|:--|:--|
| **Students** | Maintain student profiles, roll numbers, departments, CGPA, email, and contact details. |
| **Companies** | Record employers, job roles, salary information, eligibility criteria, visit dates, and hiring status. |
| **Applications** | Create applications that connect students with company opportunities and track their status. |
| **Interviews** | Schedule interview rounds and keep dates, times, and interview details together. |
| **Results** | Record placement outcomes and review result information. |
| **Accounts** | Register, log in, and log out through the account pages and servlets. |

## Recruitment workflow

1. Add student profiles and company opportunities.
2. Create applications linking students to the opportunities they are pursuing.
3. Schedule interview rounds and update application progress.
4. Record the final result so the placement team can review outcomes.

Keeping these steps connected helps a team share a consistent view of each opportunity, coordinate follow-ups, and reduce scattered or duplicated records.

## Teamwork and coordination

The system is designed around records that multiple placement team members need to reference. Student and company details provide shared context; application and interview records show progress; and results close the loop. This makes handoffs clearer and gives coordinators a common place to review the status of recruitment activity.

## Technology and structure

| Layer | Technologies |
|:--|:--|
| Web interface | JSP, HTML, CSS, JavaScript |
| Request handling | Java Servlets (Jakarta Servlet 5.0) |
| Database access | JDBC and MySQL Connector/J |
| Database | MySQL |
| Runtime | Java 17 and Apache Tomcat 10 or compatible Jakarta EE servlet container |

JSP pages render the application screens. Servlets handle requests for students, companies, applications, interviews, and results. Database access is organized through DAO classes, with model classes representing the records used by the application.

## Run the application

### Requirements

- Java 17
- MySQL 8
- Apache Tomcat 10 or another compatible Jakarta EE 9+ servlet container
- A database configured for the application

### Deploy

The repository includes a packaged web archive at `target/PlacementMS.war`. Deploy this WAR to your servlet container and open the application using the container’s local URL. For Tomcat, copy the WAR into its `webapps` directory and start the server.

Before using database-backed features, configure the application’s MySQL connection details and prepare the expected database tables. This repository does not currently include a database schema or a documented credentials file; use your local development configuration and do not commit real credentials.

## Project contents

```text
.
├── css/                 # Application styles
├── js/                  # Browser-side scripts
├── jsp/                 # JSP views for the main modules
├── WEB-INF/             # Web application configuration and compiled classes
├── META-INF/            # Application and Maven metadata
├── target/PlacementMS.war
└── README.md
```

## About the developer

Built by **Rounak Shaw**, a BCA student at **Techno India, Kolkata**, as an academic project exploring Java web development, database-backed workflows, and placement coordination.

## Connect

[Portfolio](https://rounakshaw2004.github.io/potfolio/) · [LinkedIn](https://linkedin.com/in/rounak-shaw-271a16321) · [GitHub profile](https://github.com/rounakshaw2004)
