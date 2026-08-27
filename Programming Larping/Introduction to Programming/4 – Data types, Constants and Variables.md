### 1. Why We Use Them
Programs are designed to process information. To do this, they need a way to **store, access, and modify data** in the computer's memory.
- **Variables** act as named containers for storing data values that can change during program execution.
- **Constants** act as fixed containers whose values cannot be changed once defined.
- **Data Types** specify _what kind_ of data a variable or constant can hold, ensuring the computer allocates the correct amount of memory.
### 2. Data Types in C
C provides several built-in (primitive) data types to handle different kinds of values:
- **`int` (Integers):** Used to store whole numbers (both positive and negative), without decimals.
    - _Example:_ `int age = 25;`
- **`char` (Characters):** Used to store a single character, represented using single quotes. Under the hood, characters are stored as integer ASCII values.
    - _Example:_ `char grade = 'A';`
- **`float` (Single-precision Floating-Point):** Used to store real numbers with decimal points (typically accurate up to 6 decimal places).
    - _Example:_ `float temperature = 98.6f;`
- **`double` (Double-precision Floating-Point):** Used for real numbers requiring higher precision (typically accurate up to 15 decimal places).  
    - _Example:_ `double pi = 3.1415926535;`
_Note: C also supports composite or user-defined data types (like structures, unions, and arrays) to group multiple values together._
### 3. Variables and Constants
#### Variables
A variable is a container for data values. Before using a variable in C, it **must be declared** with its data type so the compiler knows how much memory to reserve.
```C
// Declaration and Initialization
int score;       // Declaration
score = 100;     // Initialization

// Declared and initialized on the same line
float salary = 45000.50; 
```
#### Constants
Constants represent fixed values that cannot be altered by the program during its execution. They can be defined using the `const` keyword or the `#define` preprocessor directive.
```C
// Using the const keyword
const int MAX_USERS = 100;

// Using #define preprocessor directive
#define PI 3.14159
```
### 4. Operators
Operators are symbols used to perform operations on variables and values.
- **Arithmetic Operators:** Used for basic mathematical calculations.  
    - `+` (Addition), `-` (Subtraction), `*` (Multiplication), `/` (Division), `%` (Modulus/Remainder)
- **Relational & Logical Operators:** Used for comparisons and decision-making.
    - Relational: `==`, `!=`, `<`, `>`, `<=`, `>=`
    - Logical: `&&` (AND), `||` (OR), `!` (NOT)
### 5. Best Practices & Naming Rules
When naming variables and constants, follow these core rules and best practices:
- **Meaningful Identifiers:** Choose descriptive names (e.g., use `userAge` instead of just `a`).
- **Naming Rules:**
    - Variable names can contain letters, digits, and underscores (`_`).
    - They must **not** begin with a digit (e.g., `1stPlace` is invalid; `place1` is valid).
    - C is case-sensitive (`Total` and `total` are treated as two different variables).
    - You cannot use C keywords (like `int`, `return`, `float`) as variable names.