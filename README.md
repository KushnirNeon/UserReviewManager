# UserReviewManager

This project implements a **master-slave database system** in C for managing **users (master)** and their **reviews (slave)**. It provides a **file-based storage system** with **indexing, CRUD operations, and utilities** for counting and printing records. The project is designed for educational purposes to demonstrate **direct index access, file management, and relational mapping**.

---

## Features

- **Master-slave structure:**  
  - Master: Users  
  - Slave: Reviews  
- **CRUD Operations:**  
  - Insert, get, update, delete users (`insert-m`, `get-m`, `update-m`, `del-m`)  
  - Insert, get, update, delete reviews (`insert-s`, `get-s`, `update-s`, `del-s`)  
- **Indexing:**  
  - Direct access to master records using an index table  
  - Management of deleted records using garbage files  
- **Utilities:**  
  - Counting total users, total reviews, and reviews per user (`calc-m`, `calc-s`)  
  - Printing full master and slave records (`ut-m`, `ut-s`)  

---

## File Structure

| File | Purpose |
|------|---------|
| `Entities.h` | Common structs for User, Review, Indexer |
| `User.h` / `User.c` | Master file management, CRUD operations |
| `Review.h` / `Review.c` | Slave file management, CRUD operations |
| `Input.h` / `Input.c` | Functions to input Users and Reviews |
| `Output.h` / `Output.c` | Functions to print Users and Reviews |
| `Checks.h` | File and record validation functions |
| `main.c` | Command-line interface to interact with the database |
