# Problem Statement
The lack of a structured, digital system for managing books in a small library or personal collection leads to several inefficiencies:

Inaccurate Inventory: It's difficult to get a real-time count of available versus issued books, leading to accidental over-issuance or stock discrepancies.

Slow Processes: Manually searching records for book details or checking availability is time-consuming.

No Issue/Return Tracking: There is no easy way to monitor which books are currently out of the library and ensure proper return procedures are followed.

The problem is to create a simple, efficient, and reliable digital tool to streamline the inventory, issue, and return processes of a book collection.


# Scope of the Project �
The scope of this Python Library Management System is narrow and focused on core administrative functions:

In-Memory Data Storage: The system will store all book data in a global list of dictionaries that exists only while the program is running. It will not include persistent storage (like saving data to a file or database).

Book Management Only: The focus is exclusively on managing book inventory and circulation status.

Core Functionalities: The project is limited to the functionalities implemented: Add Book, Search Book, Issue Book, Return Book, and Display All.

Single-User Console Application: It operates as a command-line interface and does not include user authentication, graphical user interface (GUI), or networking capabilities.

# Target Users 
The primary users of this system are the individuals responsible for maintaining the book collection and its circulation records.

Librarians/Administrators: The staff who physically handle the books, need to update inventory, and perform the issue/return transactions.

Small Book Collection Owners: Individuals managing a personal library, a classroom library, or a small departmental book collection who need basic digital tracking.


# High-Level Features

Inventory Management:	Ability to add new books to the system with quantity and view a list of all books.
Search & Retrieval:	Capability to quickly search for a book using its unique ID.
Circulation Control:	Functions to accurately issue a book (decrementing available count) and return a book (incrementing available count).
Availability Tracking:	Automatically calculates and displays the number of available copies for any given book, preventing over-issuance.
