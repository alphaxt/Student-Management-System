
# Student Management System (C++)

A comprehensive, console-based Student Management System built in C++. This project demonstrates the practical application of fundamental **Data Structures** and **Modular Programming** principles to create, manage, and manipulate student records efficiently.

## 🚀 Features

* **Add Students:** Store detailed student profiles including Roll Number, Name, Department, Semester, CGPA, and Contact Number.
* **Display Records:** View all currently enrolled students in a clean, formatted list.
* **Search Engine:** Quickly locate a specific student by their Roll Number using an optimized Linear Search.
* **Delete Records:** Remove students from the active database.
* **Undo Delete:** Accidentally deleted a student? Instantly restore the most recently deleted profile.
* **Registration Waiting List:** Add pending students to a queue and process their official enrollment sequentially.
* **Sort Students:** View the student list sorted numerically by their Roll Number.

## 🧠 Data Structures Utilized

This project acts as a practical implementation of several core computer science data structures:

* **Singly Linked List:** Acts as the primary dynamic database. It allows the system to scale infinitely without the fixed-size limitations of standard arrays.
* **Stack (LIFO):** Powers the "Undo Delete" feature by pushing deleted nodes onto a stack and popping them back into the main list when restored.
* **Queue (FIFO):** Handles the "Registration Queue" feature, ensuring students are processed and enrolled in the exact order they applied.
* **Vectors & Bubble Sort:** Used temporarily to gather and sort student records for ordered display without disrupting the main linked list structure.

## 📂 Project Structure

The project follows standard C++ modular architecture, separating declarations from implementations for cleaner, more scalable code:

* `Student.h`: Contains the foundational `Student` class and the Linked List `Node` class.
* `StudentSystem.h`: The header file declaring the `StudentSystem` class, its variables, and function prototypes.
* `StudentSystem.cpp`: The core logic file containing the implementation of all system functions (adding, deleting, sorting, etc.).
* `main.cpp`: The entry point of the program that handles the interactive user menu and input/output.

## 🛠️ How to Compile and Run

To run this project on your local machine, you will need a standard C++ compiler (like GCC).

**1. Clone the repository:**

```bash
git clone https://github.com/YourUsername/YourRepositoryName.git
cd YourRepositoryName

```

**2. Compile the modular files together:**

```bash
g++ main.cpp StudentSystem.cpp -o StudentApp

```

**3. Run the executable:**

* **On Windows:**
```cmd
StudentApp.exe

```


* **On macOS / Linux:**
```bash
./StudentApp

```



## 🔮 Future Enhancements

* Implement File Handling (`<fstream>`) to save and load student records persistently across sessions.
* Add input validation to prevent program crashes if a user enters a letter instead of a number.
