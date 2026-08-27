### 1. Introduction to Standard I/O
Instead of hardcoding values directly into the source code, real-world programs need to interact with users dynamically. Command-line input and output allow programs to read data from the user and display results in real time using the `stdio.h` library.
### 2. The `printf` Function (Output)
`printf` is used to send formatted output to the console. It can display plain text as well as the values of variables using specific format specifiers (placeholders).
- **Common Format Specifiers:**
    - `%d` or `%i`: Integers
    - `%f`: Floating-point numbers (`float`)
    - `%lf`: Double-precision floating-point numbers (`double`)
    - `%c`: Characters
```c
#include <stdio.h>

int main() {
    int age = 22;
    float height = 5.9;
    
    // Using placeholders to output variable values
    printf("I am %d years old and %.1f feet tall.\n", age, height);
    return 0;
}
```
### 3. The `scanf` Function (Input)
`scanf` enables the program to read input entered by the user via the keyboard.
- **The Ampersand (`&`) Operator:** Unlike `printf`, `scanf` requires an ampersand before the variable name (e.g., `&age`). This passes the **memory address** of the variable rather than just a copied value.
   - **Why it matters:** Passing the memory address allows `scanf` to directly access and modify the actual value stored in that variable's memory location.
```C
#include <stdio.h>

int main() {
    int num1, num2, product;

    printf("Enter the first integer: ");
    scanf("%d", &num1); // Reads and stores input at the memory address of num1

    printf("Enter the second integer: ");
    scanf("%d", &num2); // Reads and stores input at the memory address of num2

    product = num1 * num2;
    printf("The product is: %d\n", product);

    return 0;
}
```
### 4. Summary of Key Takeaways
- **Dynamic vs. Hardcoded:** Hardcoding values requires rewriting code for new inputs. Using `scanf` and `printf` makes programs flexible and interactive.
- **Format Matching:** Ensure the format specifiers in `printf` and `scanf` match the exact data type of the variables being used (e.g., `%d` for `int`, `%f` for `float`).  
- **Memory Reference:** Always remember the `&` symbol with `scanf` for primitive variables so the program knows where to store the incoming data.