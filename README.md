Overview
The Book Notes Capstone Project is a web application designed to manage and keep track of books read, their reviews, and related notes.

Features
Book Listing: Display a list of books you've read.
Sorting: Sort books based on title, date read, or rating.
Adding New Entries: Add new book entries with details such as ISBN, title, author, description, review, and rating.
Review Update: Update book reviews.
Book Deletion: Delete books along with associated notes.
Notes Management: View, add, update, and delete notes for each book.
Technology Stack
Frontend: EJS for dynamic rendering, CSS for styling and responsiveness.
Backend: Express.js for server-side functionality.
Database: PostgreSQL for data persistence.
APIs: Open Library Covers API for fetching book cover images and Open Library Search API for book details.

How to run locally?

Clone this repository.

Navigate to the project directory.

Install dependencies using npm install.

Create a database with pgAdmin and tables 'books' and 'notes' with appropriate columns:

books table:

id (primary key)
isbn
title
author
description
review
rating
image_path
date_read
notes table:

id (primary key)
note
book_id (foreign key referencing books.id)
Create a .env file in your project directory with your database connection details:

DB_USER="your_username"
DB_HOST="your_host_address"
DB_DATABASE="your_database_name"
DB_PASSWORD="your_password"
DB_PORT="your_database_port"
Start the server using npm start.

Access the website in your browser at http://localhost:3000.
