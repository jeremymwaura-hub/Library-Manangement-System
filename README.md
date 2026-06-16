# Library Management System

## Project Description

The Library Management System is a Command Line Interface (CLI) application developed in Python. It helps users manage library operations such as viewing books, borrowing books, returning books, and tracking transactions. The system also provides administrative functionalities for managing library resources.

## Project Demonstration

Watch the project walkthrough here:

[Library Management System Demo Video]
(https://www.loom.com/share/07be4790e5d74488b1dda4722f0128c1)


## Features

### User Features

* User login and authentication
* View available books
* Borrow books
* Return books
* View transaction records

### Admin Features

* Add new books
* Update book information
* Remove books
* Manage library resources
* Access all user functionalities

## Project Structure

```text
Library-Management-System/
│
├── data/
│   ├── books.json
│   ├── users.json
│   └── transactions.json
│
├── decorators/
│   ├── auth.py
│   ├── logger.py
│   └── roles.py
│
├── models/
│   ├── user.py
│   ├── admin.py
│   ├── member.py
│   ├── book.py
│   └── transaction.py
│
├── services/
│   ├── auth_service.py
│   ├── library_service.py
│   └── storage_service.py
│
├── utils/
│   └── password_utils.py
│
├── main.py
└── README.md
```

## Data Model

### User

Attributes:

* user_name
* id
* password
* role

Methods:

* viewBook()
* borrowBook()
* returnBook()

### Admin

Inherits from User.

Additional Methods:

* addBook()
* removeBook()
* updateBook()

### Book

Attributes:

* id
* title
* author
* category
* availableCopies

Methods:

* isAvailable()
* borrowBook()
* returnBook()
* updateBook()

### Transaction

Attributes:

* trans_id
* book_id
* user_id
* action
* date

Methods:

* displayTransaction()

## Technologies Used

* Python
* JSON File Storage
* Object-Oriented Programming (OOP)
* Command Line Interface (CLI)

## Author

Developed as a Python Library Management System project by the group.
