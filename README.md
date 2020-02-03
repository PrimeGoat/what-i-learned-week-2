# What I Learned in Week 2

## Week 2 was all about JavaScript.  Below I'll review what I learned about JavaScript

- JavaScript is a scripting language that is used in websites to allow for interactive features.
- JavaScript is specified in HTML using the `<script>` tag.  It can be written inline, though it's better to specify an external javascript file using `<script src="filename.js">` so that the code can be updated from a central location.

### Comments
Comments are ignored by the JavaScript interpreter.  They are used to document code.  There are two types of commenting available in JavaScript:
- `//` - Single-line comments
- `/*`, `*/` - Multi-line comments.  Everything between `/*` and `*/` is ignored, no matter how many lines it takes up.

### Primitive data types
- Strings - A sequence of text characters that can be referenced and modified.
- Numbers - These can be integers like `1`, `32768`, and floating-point values such as `1.0`, `123.456`.
- `boolean` - A boolean value is either `true` or `false`.  This is used for logical expressions in flow control structures such as `if`/`else` conditional statements, `for`/`while` loops.
- `NaN` - Short for "Not a Number".  This type occurs during division-by-zero.
- `null` - A null value is meant to be a 'valueless' value.  This can be used if a variable's content has meaning no matter what it's set to and it needs to be set to "nothing".
- Undefined - A variable that hasn't been declared, or exists but hasn't been set to a value yet, is undefined.  Note that this is different from `null`, in that a null variable is defined and actually set to the `null`, while undefined either doesn't exist or hasn't been set yet.

### Scope
Scope is the reference frame from which variables and functions can be available from.  A variable declared within a block of code only exists within that block of code.

### Variable initialization
- `let` - Declares and optionally sets a locally-scoped variable.
```
let name = "Denis";
```
- `var` - Declares and optionally sets a globally-scoped variable.  Global variables must be used responsibly but can be very powerful and useful in the right circumstances.
```
var callCount = 0;
```
- `const` - Declares a locally-scoped constant.  A constant can only be set once, and cannot be modified after it's set.  This is to prevent accidental changes.  Constants are also treated differently by the compiler can be more efficiently referenced than variables.
```
const appName = 'TestApp';
```

### Mathematical Expressions and Operators
JavaScript allows for mathematical expressions through the use of mathematical operators.  The operator precedence and associativity is similar to that of algebra, allowing for calculations involving numbers in familiar ways.  Some of the operators in JavaScript are listed below:
- `+` - Adds two numbers or concatenates two strings
- `-` - Subtracts one number from another
- `*` - Multiplies two numbers
- `/` - Divides one number by another
- `%` - Modulus: Returns the remainder of one number divided by another
- `(`, `)` - Parentheses: Just like in algebra, parentheses are used to alter the order of operations
- `**` - Exponent: Multiplies a number to a given power

### Functions
Functions allow for code to be reused whenever needed.  A function takes an optional specified or arbitrary number of parameters as input and can return a value too.
```
function sum(a, b) {
	return a + b; // Returns the sum of a plus b
}
```

### Strings
There are many possible operations that can be done with strings.
- **Index** - A string's `n`th character can be referenced using an index using brackets (`[`, `]`).  Indexes start from `0`.
```
let firstChar = someString[0];
```
- **String Length Property** - A string's length can be checked using the `length` property as so:
```
let myString = "abc";
myString.length; // 3
```
- **Case Modification** - A string can be capitalized and un-capitalized using the `toUpperCase()` and `toLowerCase()` methods:
```
let myString = "Test String";
myString = myString.toUpperCase(); // "TEST STRING"
myString = myString.toLowerCase(); // "test string"
```
