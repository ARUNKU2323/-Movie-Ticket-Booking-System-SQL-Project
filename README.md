🎬 Movie Ticket Booking System — SQL Project

📘 Overview

This project demonstrates a Movie Ticket Booking Database System designed and implemented using Structured Query Language (SQL). It replicates the backend data structure of a real-world online movie booking platform (like BookMyShow), where users can browse movies, view show timings, make bookings, and complete payments.

The database manages multiple entities such as:

Theatres

Movies

Shows

Customers

Bookings

Payments

All tables are included in the Excel file movie_booking_basic_sql.xlsx, which can be imported into SQL databases like MySQL, PostgreSQL, or SQL Server.

🧩 Dataset Details

The Excel file consists of six interrelated tables, each representing a core entity in the movie booking system.

Table Name Description Key Columns

Theatres Stores details of all theatres and screens. Theatre_ID, Theatre_Name, Location, Total_Screens Movies Contains information about movies such as genre and duration. Movie_ID, Title, Genre, Duration, Rating Shows Represents show timings, linking movies and theatres. Show_ID, Theatre_ID, Movie_ID, Show_Date, Show_Time, Screen_No Customers Contains registered customer details. Customer_ID, Customer_Name, Email, Phone_Number Bookings Tracks ticket bookings made by customers. Booking_ID, Customer_ID, Show_ID, Seat_No, Booking_Date Payments Records transaction and payment information for each booking. Payment_ID, Booking_ID, Payment_Mode, Payment_Status, Amount

These tables are linked through primary and foreign keys to maintain referential integrity.

🧠 SQL Concepts Used

The project demonstrates fundamental to intermediate SQL concepts, including:

Database Design
Normalized schema (3NF structure)

Primary and foreign key constraints

Relationship mapping (one-to-many, many-to-one)

Data Manipulation (DML)
INSERT INTO, UPDATE, and DELETE operations

Importing data from Excel or CSV into SQL tables

Data Querying
Retrieving and filtering data using SELECT, WHERE, and ORDER BY

Using JOINs (INNER, LEFT, RIGHT) to combine tables

Applying GROUP BY and HAVING for aggregation

Analytical Queries
Finding top-grossing movies

Calculating total revenue per theatre or customer

Identifying popular show timings

Integrity & Constraints
Ensuring unique IDs with PRIMARY KEY

Maintaining relationships with FOREIGN KEY constraints

Avoiding null values using NOT NULL

⚙️ How to Use

Step 1: Create a New Database

Step 2: Create Tables

Step 3: Import Data

Step 4: Run

📊 ER Diagram (Entity Relationship)

A suggested relationship design:

Theatres (1) ────< Shows >──── (1) Movies │ │ │ │ └────< Bookings >────< Customers │ │ < Payments >

This structure ensures:

Each theatre can host multiple shows

Each movie can play in multiple theatres

Each customer can have multiple bookings

Each booking corresponds to one payment

💡 Features

Real-world movie booking data structure

Supports analytical SQL queries

Scalable for dashboard integration (Power BI, Tableau)

Clean relational schema for learning and practice

🚀 Future Enhancements

Add stored procedures for booking automation

Create triggers for payment updates

Build a front-end web interface using PHP, Python, or Node.js

Integrate with Power BI for business insights

🏷️ Author

Arunkumar V 📍Thirupathur, TamilNadu, India 📧 arunkumarbscb23@gmail.com
