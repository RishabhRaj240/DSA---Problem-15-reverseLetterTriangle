# Reverse Letter Triangle Pattern in C++

A beginner-friendly C++ program that demonstrates pattern printing using nested loops.

This project generates a **Reverse Letter Triangle Pattern**, where each row prints consecutive uppercase alphabets starting from **A**, while the number of letters decreases in each subsequent row. It is a popular pattern-printing problem from Striver's A2Z DSA Sheet and helps strengthen understanding of nested loops, character manipulation, and ASCII values.

---

## 📌 Features

* Prints a Reverse Letter Triangle Pattern
* Uses nested `for` loops
* Demonstrates character iteration using ASCII values
* Shows decreasing pattern generation
* Beginner-friendly implementation

---

## 🛠️ Technologies Used

* C++
* Standard Input/Output (`iostream`)

---

## 📂 Problem Statement

Given an integer `N`, print a reverse triangle pattern where each row contains consecutive uppercase letters starting from **A**, and the number of letters decreases by one in every row.

### Example

For:

```txt
N = 5
```

Output:

```txt
A B C D E
A B C D
A B C
A B
A
```

---

## 📸 Screenshot

<img width="1203" height="782" alt="Screenshot 2026-07-02 132503" src="https://github.com/user-attachments/assets/8bb1adc4-1ce1-4c03-844f-0b34f53900f2" />

Example folder structure:

```txt
project-folder/
│
├── main.cpp
├── README.md
└── screenshots/
    └── output.png
```

---

## 💻 Source Code

```cpp
void nLetterTriangle(int n) {
    for(int i = 0; i < n; i++) {
        for(char ch = 'A'; ch <= 'A' + (n - i - 1); ch++) {
            cout << ch << " ";
        }
        cout << endl;
    }
}
```

---

## ▶️ How to Run

1. Compile the program:

```bash
g++ main.cpp -o main
```

2. Run the executable:

```bash
./main
```

3. Enter the value of `N`.

---

## 📸 Example Output

### Input

```txt
4
```

### Output

```txt
A B C D
A B C
A B
A
```

---

## 📖 Learning Concepts

This project helps beginners understand:

* Nested loops
* Pattern printing
* Character data type (`char`)
* ASCII value manipulation
* Decreasing loop boundaries
* Algorithmic thinking

---

## 🔍 Pattern Explanation

The pattern is generated using two nested loops.

### Outer Loop

Controls the number of rows.

```cpp
for(int i = 0; i < n; i++)
```

### Inner Loop

Prints characters from **A** up to the character determined by:

```cpp
'A' + (n - i - 1)
```

As the value of `i` increases, the ending character moves backward alphabetically, resulting in one fewer letter being printed in each row.

---

## ⏱️ Complexity Analysis

### Time Complexity

```txt
O(N²)
```

The nested loops perform approximately **N²** iterations.

### Space Complexity

```txt
O(1)
```

The program uses only loop variables and does not require any additional memory.

---

## 👨‍💻 Author

Developed as a beginner-friendly C++ practice project for learning nested loops, character manipulation, and pattern printing.
