# Matrix-Operations-Program
This C program performs various matrix operations on integer, double, or complex-valued matrices. The program reads input matrices and operation commands from standard input and outputs the results of the specified operations.

Features
The program supports the following matrix operations:

ADD: Matrix addition

SUB: Matrix subtraction

MUL: Matrix multiplication

AND: Logical AND operation (for binary matrices)

OR: Logical OR operation (for binary matrices)

NOT: Logical NOT operation (for binary matrices)

TRANSPOSE: Matrix transposition

Supported Matrix Types
Integer matrices: Values are whole numbers (e.g., 1, -5, 0)

Double matrices: Values are real numbers with decimal points (e.g., 1.5, -3.2)

Complex matrices: Values are complex numbers (e.g., 1+2i, -3-4i)

Input Format
The program expects input in the following format:

Copy
(matrix1)
(matrix2 or operation)
(operation or END)
Matrix format: (rows,columns:value1,value2,...,valueN)

Example:

Copy
(2,2:1,2,3,4)
(2,2:5,6,7,8)
ADD
Output
The program outputs the resulting matrix in the same format as the input matrices, or "ERR" if an error occurs.

Error Handling
The program will output "ERR" in the following cases:

Input exceeds maximum length (128 characters)

Invalid matrix format

Operation requested on non-binary matrices for logical operations (AND, OR, NOT)

Other parsing or memory allocation errors

Compilation and Usage
Compile the program:

bash
Copy
gcc Ex3q1.c -o matrix_operations -lm
Run the program:

bash
Copy
./matrix_operations
Enter input matrices and operations as described above.

Notes
The program handles memory allocation and deallocation automatically.

For double matrices, values are rounded to one decimal place.

The program continues processing input until "END" is entered.

Example Session
Copy
(2,2:1,2,3,4)
(2,2:5,6,7,8)
ADD
(2,2:6,8,10,12)
END
Dependencies
Standard C libraries: stdio.h, stdlib.h, string.h

Complex number support: complex.h

Math library (-lm flag needed for compilation)
