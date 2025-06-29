# FILE-MANAGEMENT-TOOL
COMPANY NAME: CODETECH IT SOLUTION

NAME: ABHILASHA SHARMA

INTERN ID: CT04DF338

DOMAIN: C++

MENTOR: NEELA SANTOSH

#DISCRIPTION:
The given C++ program is a basic **File Management Tool** that allows users to interact with text files through the console. It supports three main operations: **writing new content to a file**, **reading data from a file**, and **appending additional data to an existing file**. These operations are performed using the C++ Standard Library’s file stream facilities provided by the `<fstream>` header. The program is an excellent example of how to use file I/O (Input/Output) in a structured and interactive way. This essay explains the working of the program in detail, focusing on its logic, structure, and key concepts.

---

### **Overview of File Handling in C++**

File handling in C++ is done using three classes provided in the `<fstream>` header:

1. `ofstream` – Used for writing to files.
2. `ifstream` – Used for reading from files.
3. `fstream` – Used for both reading and writing.

The program uses `ofstream` for writing and appending and `ifstream` for reading. All file streams must be checked for successful opening before operations to avoid runtime errors.

---

### **Program Structure**

The program is divided into three functions besides `main()`:

1. `writeFile(const string& filename)`
2. `readFile(const string& filename)`
3. `appendFile(const string& filename)`

Each function handles a specific file operation, making the code modular and easier to manage.

---

### **writeFile Function**

This function is responsible for **writing new data to a file**. It begins by opening the file using an `ofstream` object in default mode, which overwrites any existing content in the file. If the file fails to open, it prints an error message and exits the function.

If the file opens successfully, the function prompts the user to enter the data. It uses `cin.ignore()` to clear the input buffer, ensuring that any newline character left from previous `cin` inputs does not interfere with the upcoming `getline()` call. The user’s input is then written to the file using the `<<` operator. Finally, the file is closed, and a success message is displayed.

---

### **readFile Function**

This function is used to **read data from a file** and display it on the console. It uses an `ifstream` object to open the file in read mode. If the file cannot be opened, the function notifies the user.

Once the file is successfully opened, it reads the content line-by-line using a `while` loop and the `getline()` function. Each line is printed to the console, and the file is closed at the end. This function demonstrates efficient reading of text files line-by-line.

---

### **appendFile Function**

The third function, `appendFile`, is used to **add new content to the end of an existing file** without erasing the previous content. It uses an `ofstream` object with the `ios::app` (append) flag. If the file cannot be opened, it displays an error.

If opened successfully, the function prompts the user for input, clears the input buffer with `cin.ignore()`, and then reads the full line using `getline()`. The content is then written at the end of the file, followed by closing the stream. A confirmation message is shown to the user.

---

### **Main Function and User Interaction**

The `main()` function acts as the program's entry point and controls user interaction. It displays a menu with three options: write, read, or append. The user inputs their choice and specifies the filename.

A `switch` statement is then used to call the corresponding function based on the user's input. If an invalid choice is entered, the program outputs an "Invalid choice" message. This clear menu-driven interface makes the tool easy and intuitive to use.

---

### **Conclusion**

In summary, this C++ program demonstrates how to perform basic file operations using structured programming techniques. It highlights the importance of file stream handling, user input management, and modular function design. The use of clear prompts and error checks makes it robust and user-friendly. Though simple, this tool serves as a foundational example for building more advanced applications that involve persistent data storage.


OUTPUT:
![Image](https://github.com/user-attachments/assets/f7b3632d-4cf9-4371-97e3-31e8f9eba373)
