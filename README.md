# 🚗 Car Parking Reservation System

A simple **console-based Car Parking Reservation System developed in C++**. This project allows a parking administrator to log in, register arriving cars, view all parked cars, and calculate parking charges based on the duration of stay and VIP status.

## 📌 Project Overview

The system is designed to manage basic parking information for up to **100 cars**.

For each car, the system stores:

* Driver name
* Car number
* Hours stayed
* Time slot
* Reservation status
* VIP status

The system also provides a login system before allowing access to the main parking menu.

## ✨ Features

### 🔐 Login System

The program starts with a login screen and requires a password before accessing the parking system.

### 🚘 Car Arrival

The administrator can enter information about a newly arriving car, including driver name, car number, hours of stay, time slot, reservation status, and VIP status.

### 📋 Display Parked Cars

The system can display information about all currently parked cars.

### 💰 Calculate Parking Charges

Parking charges are calculated according to the number of hours stayed.

* VIP car → 20 rupees per hour
* Non-VIP car → 25 rupees per hour

The total charge is calculated using:

```text
Charges = Hours Stayed × Rate
```

### 🅿️ Parking Capacity

The system supports up to **100 cars**. If the maximum capacity is reached, the system displays a parking-full message.

### 🚪 Exit

The administrator can exit the program by selecting option `4`.

## 🛠️ Technologies Used

* **C++**
* Arrays
* Functions
* `if-else`
* `switch-case`
* `do-while` loop
* `for` loop
* Recursion
* Variables
* User input/output
* Boolean values
* Basic data management

## 📚 C++ Concepts Used

### Arrays

The project uses multiple arrays to store information about different cars:

```cpp
string driverNames[MAX_CARS];
int carNumbers[MAX_CARS];
double hoursStayed[MAX_CARS];
string timeSlots[MAX_CARS];
bool reserved[MAX_CARS];
bool vip[MAX_CARS];
```

Each index represents one parked car.

### Functions

The project is divided into different functions:

```text
login()
arrival()
displayAllCars()
calculateCharges()
clearScreen()
```

This makes the program easier to organize and manage.

### Switch-Case

The main menu uses `switch-case` to perform different operations based on the user's choice.

### Do-While Loop

The main menu continues to appear until the user selects option `4` to exit.

```cpp
do
{
    // menu
}
while(choice != 4);
```

### Recursion

The `login()` function calls itself when an incorrect password is entered:

```cpp
login();
```

This allows the user to try logging in again.

## ▶️ How to Run

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/Car-Parking-Reservation-System-Cpp.git
```

### 2. Open the C++ File

Open the `.cpp` file in a C++ IDE such as:

* Dev-C++
* Code::Blocks
* Visual Studio
* VS Code

### 3. Compile and Run

Compile the program and run it in the console.

## 🔑 Login

The current source code uses:

```text
Password: 123
```

## 🖥️ Main Menu

After successful login, the system displays:

```text
======CAR PARKING RESERVATION SYSTEM======

1. Arrival of a Car
2. Display All Parked Cars
3. Calculate Charges
4. Exit
```

The user selects an option to perform the required operation.

## 📂 Project Structure

```text
Car-Parking-Reservation-System-Cpp/
│
├── Car Parking system without structure.cpp
└── README.md
```

## 🎯 Learning Purpose

This project was developed as a beginner-level C++ project to practice:

* Arrays
* Functions
* Loops
* Conditional statements
* Switch-case
* Recursion
* User input/output
* Basic data management
* Simple billing calculations

## 👨‍💻 Author

**Husnain Ali**


