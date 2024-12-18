# Django Blood Donation Management System

## Overview
This Django-based project is a comprehensive Blood Donation Management System with three main features:

1. **User Registration and Appointment Booking**: Users can register or log in to book blood donation appointments. The process guides them through the necessary steps to register as a blood donor.

2. **Search for Blood Donation Centers**: Users can search for the nearest blood donation hospitals using a search feature integrated into the platform.

3. **Blog for Awareness**: A blog section allows posting articles to raise awareness about blood donation, its importance, and related topics.

### Default Login Credentials
#### Admin:
- **Username**: Hussain
- **Password**: 123

#### Sample Donor:
- **Username**: Hussain Manasi
- **Password**: 123

Alternatively, you can register a new user to test the donor functionality.

---

## Features

- **Secure User Authentication**: Users can register, log in, and manage their accounts.
- **Appointment Management**: Easily schedule and manage blood donation appointments.
- **Search Functionality**: Locate blood donation centers nearby.
- **Blog Management**: Create, read, update, and delete (CRUD) blog posts.
- **Admin Dashboard**: The admin panel enables full control of users, appointments, and blog posts.

---

# Django Blood Donation Management System

## Overview
This Django-based project is a comprehensive Blood Donation Management System with three main features:

1. **User Registration and Appointment Booking**: Users can register or log in to book blood donation appointments. The process guides them through the necessary steps to register as a blood donor.

2. **Search for Blood Donation Centers**: Users can search for the nearest blood donation hospitals using a search feature integrated into the platform.

3. **Blog for Awareness**: A blog section allows posting articles to raise awareness about blood donation, its importance, and related topics.

### Default Login Credentials
#### Admin:
- **Username**: Hussain
- **Password**: 123

#### Sample Donor:
- **Username**: Hussain Manasi
- **Password**: 123

Alternatively, you can register a new user to test the donor functionality.

---

## Features

- **Secure User Authentication**: Users can register, log in, and manage their accounts.
- **Appointment Management**: Easily schedule and manage blood donation appointments.
- **Search Functionality**: Locate blood donation centers nearby.
- **Blog Management**: Create, read, update, and delete (CRUD) blog posts.
- **Admin Dashboard**: The admin panel enables full control of users, appointments, and blog posts.

---

## How to Run

### Using Docker

1. Build the Docker image:
```bash
docker build -t blood-donation-app .
```
2. Run the Docker container:

```bash
docker run -p 8000:8000 blood-donation-app
```
Access the application at: http://localhost:8000

Command-Line Alternative
If Docker is not an option, you can run the project directly:

Install dependencies from requirements.txt:

```bash
pip install -r requirements.txt
```
Apply migrations:

```bash
python manage.py makemigrations
python manage.py migrate
```

Create a superuser if needed:

```bash
python manage.py createsuperuser
```

Run the development server:
```bash
python manage.py runserver
```
Access the application at: http://127.0.0.1:8000

Understanding Migrations
Migrations are Django’s way of propagating changes made to models (e.g., creating, updating, or deleting fields) into the database schema. Here’s how they work:

Create Migrations:

```bash
python manage.py makemigrations
```
This generates migration files based on the changes in your models.

Apply Migrations:

```bash
python manage.py migrate
```
This applies the changes to the database.

Check for Unapplied Changes: If Django detects model changes without corresponding migrations, it will display a warning when running the application. Run the above commands to resolve it.

Project Structure
The project has been divided into the following components:

1. User and Appointment Management:

    - Handles user registration, login, and appointment booking.
    - Guides users through the process of registering as a blood donor and booking their donation appointments.
    - Search Feature:

2. Allows users to find nearby blood donation centers.
    - Integrated with a simple search form for user convenience.

3. Blog:

    - A platform for posting and managing blog articles.
    - Aimed at spreading awareness about the importance of blood donation.

** Notes
Make sure the db.sqlite3 file is in the project directory to use the existing database and sample data.
Default admin and donor credentials are provided above for testing.
You can persist the database in Docker using volumes:
```bash
docker run -p 8000:8000 -v $(pwd)/db.sqlite3:/app/db.sqlite3 blood-donation-app
```
Enjoy exploring the platform, and feel free to enhance it further!

Let me know what you think!