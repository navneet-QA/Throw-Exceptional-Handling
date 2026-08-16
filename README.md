# Java Exception Handling Demystified 🚀

A structured Java repository showcasing how to handle runtime errors gracefully using standard Java Exception Handling mechanics. This project focuses on preventing application crashes and ensuring smooth data validation.

## 📌 Project Overview
This project contains clear, practical examples of how to intercept, process, and recover from exceptional conditions in Java. It covers built-in exceptions (like handling bad user inputs via `Scanner`) and demonstrates structural flow control when errors occur.

## 🛠️ Key Concepts Covered
* **Try-Catch Blocks:** Isolating risky code execution and capturing specific failure types.
* **Finally Block:** Executing cleanup code (like closing `Scanner` instances) regardless of exceptions.
* **Input Validation:** Catching `InputMismatchException` when users provide characters instead of numbers.
* **Throw vs Throws:** Explicitly generating errors and declaring them in method signatures.

## 🚀 Code Examples Included

### 1. Robust Input Validation
Prevents a program from crashing when a user types a text string into an integer-only input field:
```java
try {
    System.out.println("Enter an integer:");
    int num = sc.nextInt();
} catch (InputMismatchException e) {
    System.out.println("Invalid input! Please enter numbers only.");
}
```

### 2. Division by Zero Protection
Catching arithmetic errors safely:
```java
try {
    int result = 10 / 0;
} catch (ArithmeticException e) {
    System.out.println("Mathematical Error: Cannot divide by zero.");
}
```

## 💻 How to Run the Project
1. **Clone the repository:**
   ```bash
   git clone https://github.com
   ```
2. **Navigate to the source directory:**
   ```bash
   cd YOUR_REPOSITORY_NAME
   ```
3. **Compile the Java file:**
   ```bash
   javac YourClassName.java
   ```
4. **Execute the application:**
   ```bash
   java YourClassName
   ```

## 🛠️ Requirements
* **Java Development Kit (JDK):** Version 8 or higher
* **Terminal or IDE:** IntelliJ IDEA, Eclipse, VS Code, or Command Prompt
