# Abhay Inventory System



Name: abhay
Roll No. 2401360004
University: K.R. Mangalam University
Course: B.Tech CSE (UI/UX)
Lab: Data Structures & Algorithms (Lab) 
Course Code: ENCS253

Project Snapshot

A clean, menu-driven C++ Inventory Management System built using array-based data structures.
Designed for a grocery store scenario, this program demonstrates core array operations (insert, delete, search, display) and shows row-major/column-major views and a sparse-style low-stock representation — all as part of Lab Assignment 1: Arrays & Complexity Analysis.

Why this project?

Practical simulation of inventory operations used in retail.

Focuses on array manipulation and complexity understanding.

Lightweight, easy to read, and extendable for advanced data-structure upgrades.

Key Features

Insert Item — Add a product with ID, Name, Quantity, and Price.

Delete Item — Remove an item by its unique ID.

Search Item — Lookup by ID or Name (linear search over arrays).

Display All Items — Tabular listing of inventory contents.

Row/Column Ordering — Present Price and Quantity in row-major or column-major format.

Sparse Representation — Show items whose stock is below or equal to a user-defined threshold (helps identify rarely-restocked items).

Program Design (brief)

Storage: Fixed-size arrays of structs (Item { id, name, qty, price }).

Operations: Simple iterative algorithms suitable for array-backed collections.

Output Formats: Standard list view + matrix-style (row/column) for price/quantity + sparse list for low stock.

Time Complexity (summary)

Insert: O(1) (amortized, if space available)

Delete: O(n) (shift elements)

Search: O(n) (linear scan by ID or name)

Display: O(n)

Sparse extraction: O(n)**

# How to compile & run
g++ -std=c++17 grocery_inventory.cpp -o grocery_inventory
./grocery_inventory

Sample Run
Enter choice: 1
Enter Item ID: 101
Enter Item Name: Apple
Enter Quantity: 3
Enter Price: 50
-> Item inserted successfully.

Enter choice: 6
Enter threshold quantity for rarely restocked items: 5

--- Sparse Representation (ID | Name | Qty | Price) ---
101 | Apple | 3 | 50
