Language: CC

=== BASIC TYPES ===
int     → Integer number (e.g. 1, 42, -7)
float   → Decimal number (e.g. 3.14, -0.01)
char    → Single character (e.g. 'a', 'Z', '?')
bool    → Boolean logic value (true or false)
string  → Text consisting of multiple characters (e.g. "hello")

=== KEYWORDS & BUILT-INS ===
if          → Executes code if a condition is true
else        → Executes alternate code when "if" condition is false
while       → Repeats a block of code while a condition remains true
for         → Repeats code using a counter or iteration range
return      → Ends a function and sends back a value
printC       → Outputs a message to the console
match       → Pattern-based branching based on exact values
$use         → Imports a module or file
fun         → Declares a function (alias for clarity)
const       → Declares an unchangeable variable
struct      → Creates a custom data type with named fields

=== OPERATORS ===
\+  \-  \*  /        → Arithmetic (add, subtract, multiply, divide)
==               → Checks if two values are equal (can use `is`)
!=               → Checks if values are different
<  >  <=  >=     → Compare size or order
! (not)          → Negates a boolean (e.g. !true = false)
&& (and)         → True if both sides are true
|| (or)          → True if either side is true

=== SYNTAX ===
fun function_name(param1: type, param2: type) → return_type {
  // Function body
}

Example:
fun add(a: int, b: int) → int {
  return a + b
}

match statement:
match value {
  case 0:     // Execute if value is 0
    printC("Zero")
  case 1:
    printC("One")
  else:
    printC("Other")
}

struct definition:
struct Person {
  name: string
  age: int
}

const definition:
const max_score = 100

=== COMMENTS ===
Single-line:  // This is a comment
Multi-line :  /* This is a block comment */

=== STYLE RULES ===
- snake_case for variable and function names (e.g. max_score)
- PascalCase for struct names (e.g. UserProfile)
- Semicolons are optional (used only if multiple expressions on one line)
- No header files or includes; use `use` for modules
- Files typically use the `.ccla` extension

=== ADVANCED CONCEPTS ===
Lambda:  (x, y) => x + y   → Anonymous inline function
First-class functions → Functions can be stored in variables or passed as arguments
JSON-style objects: { "title": "CC Lang", "version": 2.0 }
