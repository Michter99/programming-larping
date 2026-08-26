### Basic C Program Structure
Every C program starts with a basic structure. In the tutorial, the instructor uses a simple text editor like Notepad to write a program that prints "Hello World" to the screen.
```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```
- **`#include <stdio.h>`:** This is a preprocessor command that tells the compiler to include the Standard Input Output library (`stdio.h`). This library is necessary to use functions like `printf`.
- **`int main()`:** This defines the main function. Every C program _must_ have a `main` function because execution always begins here.
- **`printf("...");`:** A standard library function used to print text to the console.
- **`return 0;`:** Signals to the operating system that the program executed successfully without any errors.
### Understanding Key Components
C code relies on specific syntax rules and foundational building blocks:
- **Functions:** Self-contained blocks of code that perform a specific task (e.g., `main()` and `printf()`).
- **Arguments:** The data passed into functions inside the parentheses. For example, `"Hello, World!\n"` is the argument passed to `printf`.
- **Return Values:** The output a function gives back after execution (e.g., `int main()` returns an integer value like `0`).
- **Semicolons (`;`):** Used in C to mark the end of a statement. Forgetting a semicolon will cause a compilation error.
### Compilation and Execution
Computers cannot read plain C source code directly; it must be compiled into machine code using a compiler (such as GCC).
1. **Open Command Prompt / Terminal** and navigate to the directory where your file is saved (e.g., `HelloWorld.c`).
2. **Compile the code** using GCC:
```sh
gcc HelloWorld.c -o HelloWorld.out
```
- _(If no output name is specified with `-o`, it defaults to `a.exe` on Windows or `a.out` on Linux/macOS)._
3. **Run the executable:**
	- On Windows: `HelloWorld.exe` (or `HelloWorld.exe`)        
    - On Linux/macOS: `./HelloWorld.out`
### Introduction to IDEs (Integrated Development Environments)

While basic text editors (like Notepad) work fine for small scripts, larger projects benefit from IDEs.
- **What they do:** IDEs combine a code editor, compiler, debugger, and auto-completion tools into a single application.
- **Popular examples for C:** Visual Studio, Code::Blocks, CLion, or Dev-C++.