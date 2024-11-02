# Krunal Fried Chicken (KFC) - Vulnerable Web Application
The virtual environment our group will be building revolves around having a web application with vulnerabilities in it. To do that, we will be building a website hosted on our local machine for an online food delivery service we call Krunal Fried Chicken (KFC). To build this website, we will be using regular HTML and CSS for the front-end of the website, and for the back-end. We will also be using a database to store and retrieve user data. The database management system (DBMS) we will be working on is going to be MariaDB on HeidiSQL. The IDE that will be used to write the codes for the web application is Virtual Studio Code (VSCode).

## Project Overview

- **Course**: CSEC.471.600 - Penetration Testing
- **Instructors**: Dr. Kevser Ovaz Akpinar
- **Team Members**: Krunal Thumar, Omar Jammoul, Tayyab Sajid, Khalifa Alfalasi
- **Objective**: To build a vulnerable web application and explore various web application penetration testing techniques.

- ### Prerequisites

- **Node.js** (includes npm)
- **MariaDB** (with HeidiSQL for easy management)
- **Kali Linux** VM (for testing)

### Cloning the Repository

Clone the repository to your local machine:

```
git clone https://github.com/OmarJ03/Krunal_Fried_Chicken
```

### Running the Application Locally

1. **Navigate** to the project directory:

```
cd Krunal_Fried_Chicken/KFC
```

2. **Install dependencies**:

```
npm install
```

3. **Start the application**:

```
npm run devStart
```

4. **Access the application** in your browser at:

```
http://localhost:3000
```

The application is deployed across three virtual machines:
- **Windows VM 1**: Hosts the web application.
- **Windows VM 2**: Hosts the MariaDB database.
- **Kali Linux VM**: Acts as the penetration testing environment.

## Vulnerabilities Included

The application includes the following vulnerabilities:

1. **Authentication Bypass**: SQL injection based login bypass.
2. **Sensitive Information Disclosure**: CEO's email exposed in HTML comments.
4. **Misconfigured Web Server**: Sensitive information is revealed through directory enumeration.
4. **Insecure Direct Object Reference (IDOR)**: Accessible by modifying the ID URL parameters.
5. **SQL Injection**: Exploitable using the profile page and SQLmap.
6. **Weak Password**: Easy MD5 hashcracking and weak password.

## Database Setup

1. Install MariaDB and HeidiSQL.
2. Set the default port to **3306**.
3. Import the SQL schema provided in the repository to set up the database tables and initial data.
