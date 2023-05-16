# Book Store Management System

## Introduction
This project is a Book Store Management System that allows the store clerk to efficiently manage the inventory of the book store. The system enables the clerk to perform various tasks such as entering data about new books, updating book information, deleting books from the database, and searching for the availability of books.

## Features
- User-friendly interface for easy navigation and data entry.
- Ability to add new books to the database with relevant information such as title, author, genre, and price.
- Update existing book information such as title, author, quantity, or any other relevant details.
- Remove books from the database that are no longer available or need to be deleted.
- Search functionality to quickly find books based on title, author, or any other search criteria.
- Error handling and data validation to ensure data integrity and prevent issues.

## Technologies Used
- Programming Language: [Python](https://www.python.org/)
- Database: [SQLite](https://www.sqlite.org/)

## Setup and Usage
1. Clone the repository to your local machine.
```
git clone https://github.com/your-username/book-store-management.git
```
2. Navigate to the project directory.
```
cd book-store-management
```
3. Install the required dependencies.
```
pip install -r requirements.txt
```
4. Run the application.
```
python main.py
```
5. The Book Store Management System GUI will open. From there, you can perform various actions such as adding books, updating book information, deleting books, and searching for book availability.

## Database Initialization
- The `init_db()` function is responsible for initializing the database. It checks if a table named "books" already exists in the database. If the table doesn't exist, it creates the "books" table and populates it with initial data.
- The initial data consists of four books with their respective IDs, titles, authors, and quantities. You can modify this initial data in the `books` list inside the `init_db()` function.

## Functionality
The Book Store Management System provides the following functionality:

### 1. Add Books
- The `add_books()` function allows the user to enter the ID, title, author, and quantity of a new book to be added to the database.
- The function prompts the user to input the required information and inserts the book into the "books" table in the database.
- Upon successful insertion, it displays a message confirming the addition of the book.

### 2. Update Books
- The `update_books()` function enables the user to update the information of an existing book.
- The user is prompted to enter the ID of the book they want to update and select the field they want to modify (title, author, quantity, or all fields).
- Depending on the user's selection, the function prompts for the new value(s) and updates the corresponding field(s) in the "books" table.
- After successful update, a confirmation message is displayed.

### 3. Display Database
- The `print_all_books()` function retrieves all books from the "books" table and prints their details.
- If no books are found in the database, it displays a message indicating the absence of books.
- Otherwise, it prints the ID, title, author, and quantity of each book.

### 4. Delete Books
- The `delete_books()` function allows the user to delete books from the database based on different criteria.
- The user is presented with options to delete books by ID, title, or author.
- After selecting the deletion criteria and providing the required information,
