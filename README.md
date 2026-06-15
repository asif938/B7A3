# Football Ticket Booking System Database

A relational database project for managing football fans, tournament matches, and ticket booking transactions.  
This project demonstrates database design concepts including **ERD, primary keys, foreign keys, constraints, relationships, and SQL queries**.

---

## Project Overview

The Football Ticket Booking System manages:

- Registered users (Football Fans and Ticket Managers)
- Upcoming football matches
- Ticket booking records
- Payment status tracking
- Match availability and pricing

The database ensures data consistency using relational database rules such as:

- Primary Keys
- Foreign Keys
- Unique Constraints
- Check Constraints
- Joins
- Subqueries
- Aggregate Functions

---

# Database Structure

The system contains three main tables:

## 1. Users Table

Stores information about customers and administrators.

| Column | Description |
|---|---|
| user_id | Unique user identifier (Primary Key) |
| full_name | User full name |
| email | Login email (Unique) |
| role | Football Fan / Ticket Manager |
| phone_number | Contact number |

---

## 2. Matches Table

Stores football match details.

| Column | Description |
|---|---|
| match_id | Unique match identifier (Primary Key) |
| fixture | Competing teams |
| tournament_category | League or tournament name |
| base_ticket_price | Standard ticket price |
| match_status | Availability status |

---

## 3. Bookings Table

Stores ticket purchase transactions.

| Column | Description |
|---|---|
| booking_id | Booking transaction ID (Primary Key) |
| user_id | Connected user (Foreign Key) |
| match_id | Connected match (Foreign Key) |
| seat_number | Assigned stadium seat |
| payment_status | Payment condition |
| total_cost | Final ticket cost |

---

# 🔗 Database Relationships (ERD)
