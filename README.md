# Arbitrary Precision Calculator (APC) Using&#x20;

## 📌 Project Overview

The **Arbitrary Precision Calculator (APC)** is a command-line calculator developed using C programming to perform arithmetic operations on extremely large numbers that exceed the storage capacity of standard C data types such as `int`, `long`, and `long long`.

The calculator uses a **Doubly Linked List (DLL)** data structure to represent and process large numbers. Instead of storing an entire number in a single integer variable, the number is divided into smaller segments and stored in linked-list nodes.

Arithmetic operations are implemented using custom algorithms involving digit-wise calculations, carry propagation, borrow handling, and linked-list manipulation.

This project demonstrates practical knowledge of advanced C programming, pointers, dynamic memory allocation, data structures, and algorithm development.

---

## 🎯 Project Objectives

- Develop a calculator capable of handling numbers beyond standard integer limits.
- Understand and implement Doubly Linked List data structures.
- Perform arithmetic operations without relying on built-in big-number libraries.
- Implement mathematical algorithms using pointer manipulation.
- Gain practical experience with dynamic memory allocation.
- Develop modular, reusable, and structured C programs.
- Improve problem-solving and debugging skills.

---

## ⚙️ Features

The calculator is designed to support the following arithmetic operations:

| Operator | Operation      | Description                             |
| -------- | -------------- | --------------------------------------- |
| `+`      | Addition       | Adds two large numbers                  |
| `-`      | Subtraction    | Subtracts one large number from another |
| `*`      | Multiplication | Multiplies two large numbers            |
| `/`      | Division       | Divides two large numbers               |
| `%`      | Modulus        | Calculates the remainder                |
| `^`      | Power          | Calculates exponentiation               |

**Note:** Include only the operations successfully implemented in your project.

---

## 🛠️ Technologies and Tools Used

| Category                | Technology                |
| ----------------------- | ------------------------- |
| Programming Language    | C                         |
| Data Structure          | Doubly Linked List        |
| Compiler                | GCC                       |
| Operating System        | Linux                     |
| Development Environment | Linux Terminal            |
| Memory Management       | Dynamic Memory Allocation |
| Version Control         | Git and GitHub            |

---

## 🧠 Concepts Implemented

### 1. Doubly Linked List

A Doubly Linked List is used to represent large numbers.

Each node contains:

- Data: Stores a digit or number segment.
- Previous pointer: Points to the previous node.
- Next pointer: Points to the next node.

General node representation:

```c
typedef struct node
{
    int data;
    struct node *prev;
    struct node *next;
} Node;
```

The actual node structure may vary depending on the implementation.

### 2. Dynamic Memory Allocation

Dynamic memory allocation is used to create linked-list nodes at runtime.

Functions used:

- `malloc()` – Allocates memory dynamically.
- `free()` – Releases dynamically allocated memory.

This allows the program to manage large numbers using memory as required.

### 3. Pointer Manipulation

Pointers are used to:

- Connect linked-list nodes.
- Traverse the list in forward and backward directions.
- Insert and delete nodes.
- Access and modify stored number segments.

### 4. Arithmetic Algorithm Implementation

Arithmetic operations are performed using custom algorithms rather than directly relying on standard integer arithmetic for the complete numbers.

Important concepts include:

- Carry propagation.
- Borrow handling.
- Intermediate result management.
- Sign handling.
- Division and remainder calculation.

---

## 🔢 Working Principle

The APC performs arithmetic calculations by representing large numbers using linked-list nodes.

### Step 1: Input Processing

The user provides two large numbers and an arithmetic operator.

### Step 2: Number Representation

The input numbers are processed and stored in the Doubly Linked List.

### Step 3: Operation Selection

Based on the selected operator, the corresponding arithmetic function is called.

### Step 4: Arithmetic Processing

The selected operation is performed using linked-list traversal and custom arithmetic logic.

### Step 5: Result Generation

The final result is generated and displayed on the terminal.

---

## 📂 Project Structure

The project source files are organized into separate modules for better readability and maintainability.

Example:

```text
Arbitrary-Precision-Calculator/
│
├── main.c
├── apc.h
├── addition.c
├── subtraction.c
├── multiplication.c
├── division.c
├── modulus.c
├── power.c
│
├── README.md
├── .gitignore
│
└── screenshots/
    ├── addition.png
    ├── subtraction.png
    ├── multiplication.png
    └── division.png
```

*The above structure is illustrative. Replace the filenames with your actual project files.*

---

## 💻 Installation and Execution

### Prerequisites

- Linux operating system or WSL Ubuntu.
- GCC compiler.
- Basic knowledge of C programming.

### Step 1: Install GCC

```bash
sudo apt update
sudo apt install gcc -y
```

Verify installation:

```bash
gcc --version
```

### Step 2: Clone the Repository

```bash
git clone https://github.com/vaibhavgujar8412/Arbitrary-Precision-Calculator.git
```

### Step 3: Navigate to the Project Directory

```bash
cd Arbitrary-Precision-Calculator
```

### Step 4: Compile the Source Files

If all required `.c` files are in the same directory:

```bash
gcc *.c -o apc
```

If source files are in separate directories, specify their paths.

### Step 5: Execute the Program

```bash
./apc
```

Follow the instructions displayed by the application.

---

## 🧪 Testing

The calculator should be tested with different types of inputs to verify arithmetic correctness.

Suggested test cases:

| Test Case        | Input               | Expected Purpose     |
| ---------------- | ------------------- | -------------------- |
| Small numbers    | 100 + 200           | Basic arithmetic     |
| Large numbers    | Very large operands | Precision handling   |
| Zero             | 0 + 12345           | Zero handling        |
| Equal numbers    | 500 - 500           | Zero result          |
| Different signs  | -500 + 200          | Sign handling        |
| Division         | 1000 / 10           | Quotient calculation |
| Division by zero | 100 / 0             | Error handling       |

The expected behavior depends on the operations and input cases supported by the implementation.

---

## 📚 Learning Outcomes

Through this project, I gained practical experience in:

- Advanced C programming.
- Doubly Linked List implementation.
- Dynamic memory allocation and deallocation.
- Pointer manipulation.
- Arithmetic algorithm development.
- Carry and borrow propagation.
- Modular programming.
- Debugging and problem-solving.
- Linux-based C compilation and execution.

---

## 🚀 Future Improvements

Possible enhancements include:

- Improving arithmetic algorithm efficiency.
- Adding more comprehensive input validation.
- Improving error handling.
- Supporting additional mathematical operations.
- Optimizing memory management.
- Developing a graphical user interface.

---

## 👨‍💻 Author

**Vaibhav Mahendra Gujar**

B.E. Electrical and Electronics Engineering | 2026 Graduate

**Technical Interests:** Embedded Systems, Embedded C, C Programming, Microcontrollers, and Firmware Development.

- GitHub: [vaibhavgujar8412](https://github.com/vaibhavgujar8412)
- LinkedIn: [Vaibhav Gujar](https://linkedin.com/in/vaibhav-gujar-805b32302)

---

## ⭐ Acknowledgement

This project was developed as part of the Advanced Embedded Systems Technical Training Program at Emertxe Information Technologies.

If you find this project useful, feel free to explore the source code and learn from its implementation.

**Thank you for visiting my project!**
