
# Intro_to_DB

A MySQL + Python project for designing and populating a sample online bookstore database: **`alx_book_store`**.

---

## 📚 Project Overview

The database stores:
- Books
- Authors
- Customers
- Orders
- Order details

---

## 🗂 Database Schema

### Database: `alx_book_store`

**Tables**
1. **books**
   - `book_id` (PK)
   - `title` VARCHAR(130)
   - `author_id` (FK → authors.author_id)
   - `price` DOUBLE
   - `publication_date` DATE

2. **authors**
   - `author_id` (PK)
   - `author_name` VARCHAR(215)

3. **customers**
   - `customer_id` (PK)
   - `customer_name` VARCHAR(215)
   - `email` VARCHAR(215)
   - `address` TEXT

4. **orders**
   - `order_id` (PK)
   - `customer_id` (FK → customers.customer_id)
   - `order_date` DATE

5. **order_details**
   - `orderdetailid` (PK)
   - `order_id` (FK → orders.order_id)
   - `book_id` (FK → books.book_id)
   - `quantity` DOUBLE

---

## 📂 Files in Repository

```

Intro\_to\_DB/
│── alx\_book\_store.sql   # Database creation script
│── MySQLServer.py       # Python script to create database
│── task\_2.sql           # Create all tables
│── task\_3.sql           # List all tables
│── task\_4.sql           # Full description of books table
│── task\_5.sql           # Insert single customer
│── task\_6.sql           # Insert multiple customers
└── README.md

````

---

## 🛠 Requirements
- MySQL server installed and running.
- Python 3 with MySQL connector.
- All SQL keywords in **UPPERCASE**.

---

## 🚀 Usage

**Create database**
```bash
mysql -u root -p < alx_book_store.sql
````

**Run Python database creation script**

```bash
python3 MySQLServer.py
```

**Run SQL scripts**

```bash
mysql -u root -p alx_book_store < task_2.sql
mysql -u root -p alx_book_store < task_3.sql
mysql -u root -p alx_book_store < task_4.sql
mysql -u root -p alx_book_store < task_5.sql
mysql -u root -p alx_book_store < task_6.sql
```

---

## 🎯 Learning Outcomes

* Design relational database schemas.
* Write SQL to create and manage tables.
* Connect Python to MySQL for automation.
* Insert and query data effectively.

---

**Author:** *Elaine Muhombe*
**GitHub Repository:** [Intro\_to\_DB](https://github.com/elainees-devs/Intro_to_DB)

```


