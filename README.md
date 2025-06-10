# 📚 Java Swing Library Management System

This is a **Graphical User Interface (GUI)** based **Library Management System** developed in Java using **Swing**. It enables users to add, search, borrow, and return books in a visually intuitive way. Books are categorized as **Textbooks** or **Novels**.

## 🖥️ GUI Features

- ➕ Add a new book (Textbook / Novel)
- 🔍 Search books by title
- 📖 Borrow a book
- ↩ Return a borrowed book
- 📋 View all books with their availability status

## 🧠 OOP Concepts Used

- **Abstract Class (`Book`)**: Base class for all books
- **Inheritance**: `Textbook` and `Novel` extend the `Book` class
- **Polymorphism**: Each book type provides its own version of `getInfo()`
- **Encapsulation**: Book data is managed through fields and methods

## 🛠️ Technologies Used

- Java 8 or above
- Java Swing for GUI
- ArrayList for dynamic book storage

## 📂 Project Structure

### `Book` (Abstract)
- Fields: `title`, `author`, `isBorrowed`
- Abstract Method: `getInfo()`
- Methods: `borrow()`, `returnBook()`, `getTitle()`, `isBorrowed()`

### `Textbook` (extends `Book`)
- Additional Field: `subject`
- Implements `getInfo()`

### `Novel` (extends `Book`)
- Additional Field: `genre`
- Implements `getInfo()`

### `LibraryApp`
- GUI setup with `JFrame`, `JTextField`, `JComboBox`, `JTextArea`, `JButtons`
- Event handling for all user actions
- Book list management and UI updates

## 🏁 How to Run the Program

1. Make sure you have **Java (JDK 8+)** installed.
2. Save the code in a file named `LibraryApp.java`.
3. Compile the code:
   ```bash
   javac LibraryApp.java
