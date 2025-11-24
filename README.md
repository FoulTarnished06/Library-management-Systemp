# Library-management-System

# Overview of the Project
This project implements a simple Library Management System (LMS) using Python. It's a Console-based Application that allows a librarian or administrator to manage a collection of books. The system maintains a list of books with details like ID, title, author, total quantity, and the number of issued copies. It focuses on core library operations such as adding new books, searching for specific books, issuing a book to a user, and handling book returns. All data is stored in memory (within a Python list) for the duration of the program execution.


# Features
Add Book: Allows the librarian to add a new book to the library collection, including unique ID, title, author, and initial quantity.

Search Book: Enables quick lookup of a book by its unique ID, displaying its title, author, available copies, and issued copies.

Issue Book: Records a book as issued, reducing the count of available copies, provided at least one copy is available.

Return Book: Records a book as returned, increasing the count of available copies and decreasing the issued count, provided at least one copy was issued.

Display All Books: Lists all the books currently in the library with their full details (ID, Title, Author, Total Copies, Issued, and Available).

User Menu: A simple interactive command-line interface for accessing all the functionalities.

# Technologies/Tools Used
Programming Language: Python 3

Data Structure: List of Dictionaries (used to store book records: books = [])

Input/Output: Standard Console Input (input()) and Output (print())

# Steps to Install & Run the Project
Since this is a standalone Python script, installation is minimal:

Ensure Python is Installed: Make sure you have Python 3 (version 3.6 or later recommended) installed on your operating system. You can check by running python --version or python3 --version in your terminal/command prompt.

Save the Code: Save the provided code into a file named, for example, library_management.py.

Run the Script: Open your terminal or command prompt, navigate to the directory where you saved the file, and execute the script using the following command:

Bash

python library_management.py
# OR
python3 library_management.py
The Library Management Menu will appear, and the program will begin execution.

# Instructions for Testing
Follow the steps below to test the main functionalities of the system:

Start the program by running the script.

Test 1: Add a Book (Choice 1)

Enter a unique Book ID (e.g., B001).

Enter Title (e.g., The Python Book).

Enter Author (e.g., A. Geek).

Enter Number of Copies (e.g., 5).

Verify: The message "Book added successfully!" appears.

Test 2: Display All Books (Choice 5)

Verify: The newly added book (B001) is displayed with Total Copies: 5, Issued: 0, and Available: 5.

Test 3: Issue a Book (Choice 3)

Enter the Book ID (B001).

Verify: The message "Book issued successfully!" appears.

Test 4: Search Book (Choice 2)

Enter the Book ID (B001).

Verify: The output shows Available: 4 and Issued: 1.

Test 5: Issue Maximum Available Copies

Issue the book B001 four more times.

Verify: The message "Book issued successfully!" appears after each issue.

Try to issue the book one last time. Verify: The message "No copies available!" appears.

Test 6: Return a Book (Choice 4)

Enter the Book ID (B001).

Verify: The message "Book returned successfully!" appears.

Repeat Test 4: Search for B001. Verify: The output shows Available: 1 and Issued: 4.

Test 7: Attempt to Return Excess Copies

Try returning B001 five more times.

Verify: The message "No issued copy to return!" appears when Issued reaches 0.

Test 8: Exit (Choice 6)

Verify: The message "Exiting program..." appears, and the program terminates.

