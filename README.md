# 📚 Library Book Lending System (Java Swing Desktop App)

**Course:** Object Oriented Programming (CSEG2020)  
**Semester:** IV  
**Assignment Type:** Application-Based (Take-Home)  
**Total Marks:** 30  
**Student:** Arnim Sharma (You can edit with your actual details)

---

## ✅ Overview

This is a Java-based **Library Book Lending System** with a **Graphical User Interface (GUI)** developed using **Swing**. It allows a user to manage books and members in a library, and perform lending operations with proper validations and data persistence.

---

## 🎯 Features Implemented

| Feature | Description |
|--------|-------------|
| ✅ Object-Oriented Class Design | `Book`, `Member`, `LibrarySystem` with appropriate fields and methods |
| ✅ GUI using Swing | JFrame, JButton, JTextField used to build user interface |
| ✅ View Books | Shows list of available books |
| ✅ Add Book | Add a new book with ID, title, and author |
| ✅ Register Member | Add a new member with ID and name |
| ✅ Issue Book | Issue available book to a member |
| ✅ Return Book | Return a previously issued book |
| ✅ File I/O | Saves all data in `books.txt` and `members.txt` |
| ✅ Exception Handling | Custom exceptions for unavailable books and borrow limit |
| ⭐ Bonus: History Log | Timestamped log for each lending/return using `LocalDateTime` |

---

## 🧱 Class Design Summary

- **Book**
  - Fields: `bookId`, `title`, `author`, `isAvailable`
  - Method: `displayBookInfo()` (via `toString()`)
- **Member**
  - Fields: `memberId`, `name`, `borrowedBookIds`
  - Methods: `borrowBook()`, `returnBook()`
- **LibrarySystem**
  - Holds lists of books and members
  - Methods: add book/member, issue/return books, file load/save

---

## 🖼️ Sample Screenshots

> 📸 *Include screenshots of:*
- The main GUI window
- Add book/member popup
- Book issue and return confirmations

---

## 🚀 How to Run the Project

### ✅ Prerequisites
- Java JDK 17+ installed
- VS Code (or any Java IDE)
- Java Extension Pack (in VS Code)

### ▶️ Steps

1. Clone or download the project folder
2. Open in VS Code
3. Ensure these files exist:
   - `Book.java`, `Member.java`, `LibrarySystem.java`, `LibraryGUI.java`
   - `BookNotAvailableException.java`, `MaxLimitReachedException.java`
   - `books.txt`, `members.txt` (empty files in same folder)
4. Compile and run:

```bash
javac *.java
java LibraryGUI
