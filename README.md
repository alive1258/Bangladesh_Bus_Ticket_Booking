# 🚌 Bangladesh Bus Ticket Booking System

A simple console-based **Bus Ticket Booking System** developed using **Python Object-Oriented Programming (OOP)**. This project allows users to view available buses, book tickets, and manage buses through an admin panel.

## 📌 Project Overview

The Bangladesh Bus Ticket Booking System is designed to demonstrate core Object-Oriented Programming concepts in Python.

The system provides separate menus for regular users and administrators. Users can view available buses and book tickets, while administrators can log in and manage bus information.

### OOP Concepts Used

- Classes and Objects
- Constructors (`__init__`)
- Encapsulation
- Object Relationships
- Methods and Attributes
- Conditional Statements
- Loops
- Input Validation
- Object References

## ✨ Features

### 👤 User Features

- View all available buses.
- Check available seats for each bus.
- Book bus tickets.
- Enter passenger name and phone number.
- Receive booking confirmation.
- Fixed ticket fare of **৳500**.
- Get feedback when a bus is fully booked or unavailable.

### 🔐 Admin Features

- Admin login using predefined credentials.
- Add new buses to the system.
- View all registered buses.
- Check available seats.
- Logout from the admin panel.

## 🔑 Admin Login Credentials

| Field    | Value   |
| -------- | ------- |
| Username | `admin` |
| Password | `1234`  |

> Note: These are predefined credentials for this academic project.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Programming Paradigm:** Object-Oriented Programming (OOP)
- **Interface:** Command-Line Interface (CLI)
- **External Libraries:** None

## 📂 Project Structure

```text
Bangladesh-Bus-Ticket-Booking-System/
│
├── main.py           # Main application and menu system
├── bus.py            # Bus class and seat management
├── passenger.py      # Passenger class and information
├── bus_system.py     # Bus management and ticket booking
├── admin.py          # Admin authentication
└── README.md         # Project documentation
```

## 🧩 Project Modules & OOP Classes

### 1. `bus.py` — Bus Class

Manages individual bus information and seat availability.

**Attributes:**

- `number` – Bus number.
- `route` – Bus route.
- `total_seats` – Total number of seats.
- `booked_seats` – Number of booked seats (default: 0).

**Methods:**

- `available_seats()` – Returns the number of available seats.
- `book_seat()` – Books a seat if one is available.

### 2. `passenger.py` — Passenger Class

Stores passenger details and their selected bus.

**Attributes:**

- `name` – Passenger name.
- `phone` – Passenger phone number.
- `bus` – Reference to the selected Bus object.

### 3. `bus_system.py` — BusSystem Class

Handles the main bus management and ticket booking operations.

**Attributes:**

- `buses` – List of registered buses.
- `passengers` – List of passenger bookings.

**Methods:**

- `add_bus(number, route, seats)` – Adds a new bus to the system.
- `book_ticket(bus_number, name, phone)` – Finds a bus, checks seat availability, books a ticket, and creates a passenger record.
- `show_buses()` – Displays all registered buses and their available seats.

### 4. `admin.py` — Admin Class

Manages administrator authentication.

**Attributes:**

- `username` – Admin username.
- `password` – Admin password.

**Method:**

- `login()` – Validates administrator login credentials.

**Default Credentials:**

| Field    | Value   |
| -------- | ------- |
| Username | `admin` |
| Password | `1234`  |

### 5. `main.py` — Main Application

Runs the application and manages the complete menu system.

**Responsibilities:**

- Displays the main user menu.
- Handles admin login.
- Displays the admin menu after successful login.
- Allows administrators to add new buses.
- Allows users to book tickets.
- Displays available buses.
- Handles logout and application exit.

## 🚀 Installation & Run

Follow these steps to run the project on your computer.

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/Bangladesh-Bus-Ticket-Booking-System.git
```

### Step 2: Navigate to the Project Directory

```bash
cd Bangladesh-Bus-Ticket-Booking-System
```

### Step 3: Check Python Installation

```bash
python --version
```

Python 3 is recommended.

### Step 4: Run the Application

```bash
python main.py
```

**Note:** No external Python packages are required.

## 📋 Application Menu

### 👤 User Menu

The main menu is accessible to everyone.

```text
========================================
   BANGLADESH BUS TICKET BOOKING SYSTEM
========================================

1. Admin Login
2. Book Ticket
3. View Buses
4. Exit

Enter your choice:
```

### 🔐 Admin Menu

Only administrators with valid login credentials can access this menu.

```text
========================================
              ADMIN MENU
========================================

1. Add Bus
2. View All Buses
3. Logout

Enter your choice:
```

## 💰 Fixed Ticket Fare

Each successfully booked ticket costs **৳500**.

| Item       | Amount |
| ---------- | -----: |
| Per Ticket |   ৳500 |

## ✅ Input Validation & User Feedback

The system is designed to handle common input and booking situations:

- Invalid menu choices.
- Incorrect admin login credentials.
- Non-existent bus numbers.
- Fully booked buses.
- Invalid passenger information.
- Attempts to book tickets when no seats are available.
- Successful bus registration.
- Successful ticket booking.
- Admin logout confirmation.

## 🔄 System Workflow

1. Start the application using `main.py`.
2. Select an option from the main menu.
3. View available buses or book a ticket.
4. To manage buses, select Admin Login.
5. Enter the admin username and password.
6. After successful login, access the Admin Menu.
7. Add buses or view all registered buses.
8. Logout to return to the main menu.
9. Select Exit to close the application.

## 👨‍💻 Author

**Zamirul Kabir**

## 📄 License

This project is created for educational and academic purposes.
