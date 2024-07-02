
## Here's a detailed GitHub README for your Contact Book project, including key features and project details:

## Contact Book Project
This project is a simple Contact Book application implemented in Python using Object-Oriented Programming (OOP) concepts. The application provides a menu-driven interface for users to add, display, and search for contacts.

## Key Features
Add Contact: Allows you to add a new contact to the contact book.
Display All Contacts: Displays all contacts stored in the contact book.
Search Contact: Allows you to search for a contact by name.
Exit: Exits the application.


## Project Structure
contact.py: Defines the Contact class.
contact_book.py: Defines the ContactBook class.
main.py: Contains the main program logic and menu.


## Classes
Contact
The Contact class represents a single contact with a name and phone number.

python
Copy code
class Contact:
    def __init__(self, name, phone):
        self.name = name
        self.phone = phone

    def __str__(self):
        return f"Name: {self.name}, Phone: {self.phone}"
## ContactBook
The ContactBook class manages a collection of Contact instances and provides methods to add, display, and search for contacts.
python
Copy code
class ContactBook:
    def __init__(self):
        self.contacts = []

    def add_contact(self, contact):
        self.contacts.append(contact)

    def display_contacts(self):
        for contact in self.contacts:
            print(contact)

    def search_contact(self, name):
        for contact in self.contacts:
            if contact.name == name:
                print(contact)
                return
        print("Contact not found.")

## Getting Started
Prerequisites
Python 3.x
Installation
Clone the repository:
bash
Copy code
git clone https://github.com/yourusername/contact-book.git
cd contact-book
Run the application:
bash
Copy code
python main.py

## Usage

Add Contact: Follow the prompts to add a new contact by entering the contact's name and phone number.
Display All Contacts: Choose this option to view all contacts stored in the contact book.
Search Contact: Enter the name of the contact you wish to search for.
Exit: Exit the application.
Example
plaintext
Copy code
Contact Book Menu:
1. Add Contact
2. Display All Contacts
3. Search Contact
4. Exit
Enter your choice (1/2/3/4): 1
Enter name: John Doe
Enter phone: 1234567890
Contact added successfully!

Contact Book Menu:
1. Add Contact
2. Display All Contacts
3. Search Contact
4. Exit
Enter your choice (1/2/3/4): 2
Name: John Doe, Phone: 1234567890

Contact Book Menu:
1. Add Contact
2. Display All Contacts
3. Search Contact
4. Exit
Enter your choice (1/2/3/4): 3
Enter name to search: John Doe
Name: John Doe, Phone: 1234567890

Contact Book Menu:
1. Add Contact
2. Display All Contacts
3. Search Contact
4. Exit
Enter your choice (1/2/3/4): 4
Exiting...
