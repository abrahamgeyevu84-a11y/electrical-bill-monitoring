# Electrical Load Monitoring System

A simple C++ console-based application that helps users monitor household electrical appliances, calculate daily energy consumption, and estimate electricity bills.

This project demonstrates file handling, structures, vectors, and basic billing calculations in C++.

---

## Features

- Register new electrical appliances
- View all registered appliances
- Search for an appliance by name
- Calculate daily and estimated monthly electricity cost
- Save appliance data to file
- Save billing summaries with date and time
- Persistent storage using text files

---

## How It Works

Each appliance stores:

- Name
- Power rating (watts)
- Hours used per day

Energy consumption formula:

kWh per day = (Watts / 1000) × Hours used

Billing formulas:

Daily Cost = Total kWh × Tariff  
Monthly Cost = Daily Cost × 30  

---

## File Storage

The program uses two files:

appliances.txt  
Stores all registered appliances in this format:

Name|Watts|Hours

Example:

Fan|75|8  
Television|120|5  

billing_summary.txt  
Stores saved billing reports with timestamps.

---

## Menu Options

1. Register Appliance  
2. View Appliances  
3. Search Appliance  
4. Calculate Bill  
5. Save Appliances  
6. Exit  

Appliances are automatically saved when exiting the program.

---

## Requirements

- C++ compiler (G++, MinGW, or any standard C++ compiler)
- C++11 or later

---

## How to Compile and Run

Using g++:

g++ main.cpp -o load_monitor  
./load_monitor  

On Windows:

g++ main.cpp -o load_monitor.exe  
load_monitor.exe  

---

## Project Structure

.
├── main.cpp  
├── appliances.txt  
├── billing_summary.txt  
└── README.md  

---

## Concepts Used

- Structures (struct)
- Vectors (std::vector)
- File handling (ifstream, ofstream)
- Time handling (ctime)
- Loops and conditionals
- Formatted output (iomanip)

---

## Purpose

This project is suitable for beginners learning C++.  
It helps in understanding file handling and basic energy consumption calculations.  
It can also be used as a simple academic mini project.

---

## Author

C++ Electrical Load Monitoring System