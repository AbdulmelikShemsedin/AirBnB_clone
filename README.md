AirBnB Clone - The Console
This project is the first step of the AirBnB Clone. It aims to replicate the core functionality of the AirBnB web app, starting with a powerful command-line interface (CLI) that handles the backend of the app through a custom shell known as the Console.

It is built in Python and uses the OOP (Object-Oriented Programming) approach to manage objects such as users, places, reviews, and more — which will eventually be stored in a database and displayed in a frontend.

======================================================================


=====================================================================
 Project Description
This version of the project focuses on:

Creating a custom command interpreter that works like a shell.

Managing objects through commands like create, show, destroy, all, and update.

Storing and retrieving data from a JSON file using file serialization/deserialization.

Implementing the base model and other classes like User, Place, Review, City, Amenity, and State.
=====================================================================


=====================================================================
 The Command Interpreter
 How to Start the Console
 code
./console.py
Once inside the console, it runs in interactive mode.

To exit:
Press Ctrl+D or
Type quit

To run in non-interactive mode:

code
echo "help" | ./console.py


=====================================================================



======================================================================
 How to Use
Once the console is running, you can use the following commands:

Command	Description
help	Shows help on available commands
create <class>	Creates a new instance of a class and prints the ID
show <class> <id>	Prints the string representation of an instance
destroy <class> <id>	Deletes an instance
all [<class>]	Prints all string representations of all instances or class-specific
update <class> <id> <attribute> <value>	Updates an instance with new attribute values

======================================================================





======================================================================
 Examples
code
(hbnb) create User
b6a6e15c-28d1-4b80-94a5-87d0dc0b61c3

(hbnb) show User b6a6e15c-28d1-4b80-94a5-87d0dc0b61c3
[User] (b6a6e15c...) {'id': 'b6a6e15c...', 'created_at': ..., ...}

(hbnb) all
["[User] (b6a6e15c...) {...}", "[BaseModel] (...)", ...]

(hbnb) update User b6a6e15c... first_name "John"
(hbnb) show User b6a6e15c...
[User] (...) {'id': ..., 'first_name': 'John', ...}

(hbnb) destroy User b6a6e15c...
(hbnb) all User
[]



