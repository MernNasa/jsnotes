# What is javascript ?
JavaScript is a high-level, interpreted (JIT-compiled), dynamically typed, single-threaded, multi-paradigm programming language used to build interactive web applications. It runs in browsers and also on servers through environments like Node.js.

# JavaScript Features 

1. Lightweight
2. Interpreted (JIT-compiled)
3. Dynamically typed
4. Loosely (weakly) typed
5. Single-threaded
6. Synchronous by default, with asynchronous support (callbacks, promises, async/await)
7. Prototype-based
8. Object-oriented
9. Scripting language
10. Runs on both client (browser) and server (Node.js)

# Another Definition for JS
JavaScript is a lightweight, interpreted (JIT-compiled), dynamically typed,
loosely typed, prototype-based, object-oriented scripting language.
It is single-threaded and synchronous by default, but supports asynchronous
programming using callbacks, promises, and async/await.
It runs in the browser and on the server (Node.js).


# What is Scripting Language?
A scripting language is a programming language that is interpreted at runtime (line by line or via JIT) instead of being compiled into a separate executable file beforehand. It is mainly used to automate tasks and add behavior to existing applications.

Ex: JavaScript, Python, PHP

# Key Points
1. Code is executed by an interpreter or runtime engine (no separate compile step)
2. Usually used to control or automate another application (e.g., a web browser)
3. Generally easy to learn and quick to write
4. Typically dynamically typed
5. Runs inside a host environment (browser, Node.js)

# What is programming language ?

A programming language is a formal language with a set of rules (syntax) and instructions used to write programs that tell a computer what to do. The code is translated by a compiler or interpreter into machine code (0s and 1s) that the computer can execute.

1. Low-level----Machine language, Assembly
2. High-level-----JavaScript, Python, Java


# Programming Language vs Scripting Language
1. Every scripting language is a programming language.
2. Not every programming language is a scripting language.
3. Scripting languages are usually interpreted and used to automate tasks.
4. Programming languages can be compiled or interpreted and are used to build complete applications.


# Server-Side Rendering (SSR) vs Client-Side Rendering (CSR)

| Feature | Server-Side Rendering (SSR) | Client-Side Rendering (CSR) |
|---|---|---|
| **Definition** | HTML is generated on the server and sent to the browser as a ready-to-display page | Browser receives a minimal HTML file and JavaScript builds the page in the browser |
| **Where rendering happens** | Server | Browser (client) |
| **Initial page load** | Faster (content is ready on arrival) | Slower (must download and run JS first) |
| **Subsequent navigation** | Slower (often requests a new page from the server) | Faster (only data is fetched, no full reload) |
| **SEO** | Excellent (crawlers get full HTML) | Weaker (content depends on JS execution), though modern crawlers handle it better |
| **Server load** | High (server renders every request) | Low (browser does the work) |
| **Client device load** | Low | High (depends on user's device) |
| **Interactivity** | Needs hydration before the page becomes interactive | Interactive once JS finishes loading |
| **Best for** | Blogs, e-commerce, news sites, marketing pages | Dashboards, web apps, SPAs, admin panels |
| **Caching** | Harder for dynamic pages (easier with CDN for static output) | Easy (static files cached on CDN) |
| **Social media previews** | Works well (meta tags in HTML) | Poor unless extra setup is done |
| **Examples / Tools** | Next.js (SSR), Nuxt.js, Remix, PHP, Django templates | React (CRA), Vue, Angular (default SPA setup) |
| **Page flow** | Request → Server builds HTML → Browser shows page → Hydration | Request → Empty HTML + JS bundle → JS runs → Browser builds page |



# What is Tokens ?
A token is the smallest meaningful unit of a JavaScript program. When the JS engine reads your code, it first breaks it into tokens (this step is called lexical analysis or tokenization) before parsing and executing it.

# Types of Tokens
1. Keywords        -> let, const, if, function, return
2. Identifiers     -> variable and function names (a, userName, getData)
3. Literals        -> 20, "hello", true, null
4. Operators       -> +, -, =, ===, &&
5. Punctuators     -> ( ) { } [ ] ; , .
6. Template tokens -> `Hello ${name}`


Ex: let a = 20;
let   -> keyword
a     -> identifier
=     -> operator
20    -> literal
;     -> punctuator

# What is Keywords?
Keywords are reserved words in JavaScript that have a predefined meaning for the language. They are used to perform specific actions or define the structure of a program, and they cannot be used as variable, function, or identifier names.

Ex: break, case, catch, class, const, continue, debugger, default, delete,
do, else, export, extends, finally, for, function, if, import, in,
instanceof, new, return, super, switch, this, throw, try, typeof,
var, while, null, true, false

# Note
 JavaScript has around 36 core reserved keywords. so the total is roughly 50+ depending on the ECMAScript version


# what is an identifier ?
An identifier is the name given to a variable, function, class, object property, label, or parameter so that it can be referred to later in the program.

# Rules for Identifiers
1. Must start with a letter (a-z, A-Z), underscore (_), or dollar sign ($)
2. After the first character, it can contain letters, digits (0-9), _ or $
3. Cannot start with a digit
4. Cannot contain spaces
5. Cannot contain special characters like @, #, %, -, +, etc. (other than _ and $)
6. Cannot be a reserved keyword (let, if, for, class, etc.)
7. Case sensitive (name, Name, and NAME are different identifiers)
8. No length limit
9. Can use Unicode letters (e.g., let café = 1;)

# What is an Operator ?
An operator is a symbol or keyword that performs an operation on one or more values (called operands) and produces a result.

# Types of Operators
1. Arithmetic Operators (+,-,*,/,%,**,++,--)
2. Assignment Operators(=,+=,-=,*=,/=,%=,**=)
3. Comparison Operators(==,===,>,<,>=,<=,!=,!==)
4. Logical Operators(&&,||,!)

# What is a literal?
A literal is a fixed value written directly in the source code. It represents the value itself, not a variable or an expression that computes it.

# What is Datatype in JS?
A data type defines the kind of value a variable can hold and what operations can be performed on it. JavaScript is dynamically typed, so the type is decided at runtime and can change.

# Types of Data Types

JavaScript has two categories:
1. Primitive (7 types)
2. Non-primitive / Reference (Object)

# 1. Primitive (7 types)
1. String
2. Number
3. Boolean
4. undefined
5. null
6. bigint
7. symbol

# 2. Non-primitive / Reference (Object)

1. Arrays
2. Object
3. function

# What is Conditional Statements in JavaScript?
Conditional statements are used to make decisions in a program. They execute a block of code only if a specified condition is true (or falsy/truthy), allowing the program to follow different paths.

# Types of Conditional Statements
1. if
2. if...else
3. if...else if...else
4. switch
5. Ternary operator (? :)
6. Nested if


# Conditional Statements in JavaScript

## 1. if Statement

Runs the block only if the condition is true.

```js
let age = 20;
if (age >= 18) {
  console.log("Adult");
}
```

## 2. if...else Statement

```js
let age = 15;
if (age >= 18) {
  console.log("Adult");
} else {
  console.log("Minor");
}
```

## 3. if...else if...else Statement

Used when there are multiple conditions.

```js
let marks = 75;
if (marks >= 90) {
  console.log("Grade A");
} else if (marks >= 60) {
  console.log("Grade B");
} else {
  console.log("Grade C");
}
```

## 4. switch Statement

Compares one value against many cases (uses strict comparison `===`).

```js
let day = 2;
switch (day) {
  case 1:
    console.log("Monday");
    break;
  case 2:
    console.log("Tuesday");
    break;
  default:
    console.log("Invalid day");
}
```

> **Note:** `break` stops execution from falling through to the next case.

## 5. Ternary Operator

Short form of `if...else`.

```js
let result = age >= 18 ? "Adult" : "Minor";
```

## 6. Nested if

An `if` inside another `if`.

```js
if (age >= 18) {
  if (hasID) {
    console.log("Allowed");
  }
}
```



# What is loops in JS
A loop is a control flow statement that executes a block of code repeatedly as long as a specified condition is true. Loops save time and avoid writing the same code again and again.

Ex: 
```js
      // Without a loop
      console.log(1);
      console.log(2);
      console.log(3);
      
      // With a loop
      for (let i = 1; i <= 3; i++) {
        console.log(i);
      }

```

# Types of Loops
1. for
2. while
3. do...while
4. for...in
5. for...of

# Loops in JavaScript

## 1. `for` Loop

Used when you know how many times to repeat.

```js
for (let i = 1; i <= 5; i++) {
  console.log(i);
}
```

**Syntax:**

```
for (initialization; condition; increment/decrement) {
  // code
}
```

## 2. `while` Loop

Checks the condition **first**, then runs. Used when the number of repetitions is not known.

```js
let i = 1;
while (i <= 5) {
  console.log(i);
  i++;
}
```

## 3. `do...while` Loop

Runs the code **at least once**, then checks the condition.

```js
let i = 10;
do {
  console.log(i);   // prints 10 even though the condition is false
  i++;
} while (i <= 5);
```

## 4. `for...in` Loop

Loops over the **keys (property names)** of an object.

```js
let user = { name: "Ravi", age: 25 };
for (let key in user) {
  console.log(key, user[key]);
}
// name Ravi
// age 25
```

> **Note:** Avoid using `for...in` on arrays (it gives indexes as strings and may include inherited properties).

## 5. `for...of` Loop

Loops over the **values** of iterable objects like arrays, strings.

```js
let fruits = ["apple", "banana", "mango"];
for (let fruit of fruits) {
  console.log(fruit);
}
```


## Classification

| Type | Loops | Condition checked |
|---|---|---|
| **Entry-controlled** | `for`, `while` | Before running the body |
| **Exit-controlled** | `do...while` | After running the body |


## `for...in` vs `for...of`

| Feature | `for...in` | `for...of` |
|---|---|---|
| **Gives** | Keys / indexes | Values |
| **Works on** | Objects (enumerable properties) | Iterables (arrays, strings, Maps, Sets) |
| **Plain objects** | Yes | No (objects are not iterable) |



# What is a Function in JS?
A function is a reusable block of code that performs a specific task. It runs only when it is called (invoked), can accept inputs (parameters), and can return an output.

```js
function add(a, b) {
  return a + b;
}

console.log(add(2, 3)); // 5

```
# Function Terminology
1. Function name -> add
2. Parameters    -> a, b (placeholders in the definition)
3. Arguments     -> 2, 3 (actual values passed when calling)
4. Return value  -> the result sent back using return
5. Function call -> add(2, 3)


# Types of Functions
1. Named Function
2. Anonymous Function
3. Function Expression
4. Arrow Function
5. IIFE (Immediately Invoked Function Expression)
6. Higher-Order Function
7. Callback Function
8. Generator Function
9. Pure Function
10. Async Function
11. Recursive Function

# Types of Functions in JavaScript

## 1. Named Function

A function that has a name. It is created using the `function` keyword and can be called before it is defined (hoisting).

```js
function greet(name) {
  return "Hello " + name;
}

console.log(greet("Ravi")); // Hello Ravi
```

## 2. Anonymous Function

A function without a name. It is usually used as a value or passed as an argument.

```js
setTimeout(function () {
  console.log("Hi");
}, 1000);
```

## 3. Function Expression

A function stored inside a variable. It can be called only after the line where it is defined (not hoisted).

```js
const add = function (a, b) {
  return a + b;
};

console.log(add(2, 3)); // 5
```

## 4. Arrow Function

A shorter syntax for writing functions (ES6). It does not have its own `this` and cannot be used as a constructor.

```js
const square = (x) => x * x;

console.log(square(4)); // 16
```

## 5. IIFE (Immediately Invoked Function Expression)

A function that runs immediately after it is defined. It is used to avoid polluting the global scope.

```js
(function () {
  console.log("Runs immediately");
})();
```

## 6. Higher-Order Function

A function that takes another function as an argument or returns a function.

```js
const numbers = [1, 2, 3];
const doubled = numbers.map((n) => n * 2);

console.log(doubled); // [2, 4, 6]
```

## 7. Callback Function

A function passed as an argument to another function, to be executed later.

```js
function process(callback) {
  console.log("Processing...");
  callback();
}

process(() => console.log("Done"));
// Processing...
// Done
```

## 8. Generator Function

A function that can pause and resume its execution using `yield`. It is defined with `function*`.

```js
function* count() {
  yield 1;
  yield 2;
  yield 3;
}

const gen = count();
console.log(gen.next().value); // 1
console.log(gen.next().value); // 2
```

## 9. Pure Function

A function that always returns the same output for the same input and has no side effects (does not change outside variables).

```js
function add(a, b) {
  return a + b;
}

console.log(add(2, 3)); // 5
```

## 10. Async Function

A function declared with `async` that always returns a promise and allows the use of `await` inside it.

```js
async function getData() {
  const res = await fetch("https://jsonplaceholder.typicode.com/todos/1");
  const data = await res.json();
  return data;
}

getData().then((data) => console.log(data));
```

## 11. Recursive Function

A function that calls itself until a stopping condition (base case) is met.

```js
function factorial(n) {
  if (n <= 1) return 1;   // base case
  return n * factorial(n - 1);
}

console.log(factorial(5)); // 120
```

## Summary Table

| Function Type | Key Point |
|---|---|
| Named Function | Has a name, hoisted |
| Anonymous Function | No name |
| Function Expression | Stored in a variable, not hoisted |
| Arrow Function | Short syntax, no own `this` |
| IIFE | Runs immediately |
| Higher-Order Function | Takes or returns a function |
| Callback Function | Passed as an argument, runs later |
| Generator Function | Pauses and resumes with `yield` |
| Pure Function | Same input, same output, no side effects |
| Async Function | Returns a promise, uses `await` |
| Recursive Function | Calls itself |


# String Built-in Methods in JavaScript
# Property
1. length

# Character Access
2. charAt()
3. charCodeAt()
4. at()


# Searching
5. indexOf()
6. lastIndexOf()
7. includes()
8. startsWith()
9. endsWith()
10. search()
11. match()
12. matchAll()

# Extracting
13. slice()
14. substring()
15. substr() (deprecated)

# Modifying / Transforming
16. toUpperCase()
17. toLowerCase()
18. trim()
19. trimStart()
20. trimEnd()
21. padStart()
22. padEnd()
23. repeat()
24. replace()
25. replaceAll()
26. concat()
27. split()

# Comparison
28. localeCompare()

# Conversion
29. toString()

# Static Methods
30. String.fromCharCode()



# String Built-in Methods in JavaScript

> Strings are **immutable**. Every method returns a **new value** and never changes the original string.

---

## Property

### 1. `length`

Returns the number of characters in the string. It is a property, so there are no parentheses.

- **Accepts:** nothing
- **Returns (condition matches):** the number of characters (number)
- **Returns (no match):** `0` for an empty string

```js
"Hello".length;  // 5
"".length;       // 0
```

---

## Character Access

### 2. `charAt(index)`

Returns the character at the given index.

- **Accepts:** `index` (number, default `0`)
- **Returns (match):** the character at that index
- **Returns (no match):** `""` (empty string) if the index is out of range

```js
"Hello".charAt(1);   // "e"
"Hello".charAt(10);  // ""
```

### 3. `charCodeAt(index)`

Returns the UTF-16 character code at the given index.

- **Accepts:** `index` (number, default `0`)
- **Returns (match):** a number (0 to 65535)
- **Returns (no match):** `NaN` if the index is out of range

```js
"A".charCodeAt(0);     // 65
"Hello".charCodeAt(10); // NaN
```

### 4. `at(index)`

Returns the character at the given index. It supports **negative indexes** (counting from the end).

- **Accepts:** `index` (number, can be negative)
- **Returns (match):** the character at that index
- **Returns (no match):** `undefined` if the index is out of range

```js
"Hello".at(1);    // "e"
"Hello".at(-1);   // "o"
"Hello".at(10);   // undefined
```

---

## Searching

### 5. `indexOf(searchString, position)`

Returns the index of the **first** occurrence of the text.

- **Accepts:** `searchString` (string), `position` (optional start index)
- **Returns (match):** the index of the first occurrence (number)
- **Returns (no match):** `-1`

```js
"hello world".indexOf("o");   // 4
"hello world".indexOf("z");   // -1
```

### 6. `lastIndexOf(searchString, position)`

Returns the index of the **last** occurrence of the text.

- **Accepts:** `searchString` (string), `position` (optional, searches backward from here)
- **Returns (match):** the index of the last occurrence
- **Returns (no match):** `-1`

```js
"hello world".lastIndexOf("o");  // 7
"hello world".lastIndexOf("z");  // -1
```

### 7. `includes(searchString, position)`

Checks whether the string contains the given text.

- **Accepts:** `searchString` (string), `position` (optional start index)
- **Returns (match):** `true`
- **Returns (no match):** `false`

```js
"hello world".includes("world");  // true
"hello world".includes("abc");    // false
```

> Throws a `TypeError` if you pass a regular expression.

### 8. `startsWith(searchString, position)`

Checks whether the string starts with the given text.

- **Accepts:** `searchString` (string), `position` (optional index to start checking from)
- **Returns (match):** `true`
- **Returns (no match):** `false`

```js
"JavaScript".startsWith("Java");  // true
"JavaScript".startsWith("Script"); // false
```

### 9. `endsWith(searchString, endPosition)`

Checks whether the string ends with the given text.

- **Accepts:** `searchString` (string), `endPosition` (optional, treats the string as this long)
- **Returns (match):** `true`
- **Returns (no match):** `false`

```js
"JavaScript".endsWith("Script");  // true
"JavaScript".endsWith("Java");    // false
```

### 10. `search(regexp)`

Searches for a match using a regular expression and returns its index.

- **Accepts:** a regular expression (or a string, which is converted to a regex)
- **Returns (match):** the index of the first match
- **Returns (no match):** `-1`

```js
"hello 123".search(/\d/);   // 6
"hello".search(/\d/);       // -1
```

### 11. `match(regexp)`

Finds matches of a regular expression in the string.

- **Accepts:** a regular expression
- **Returns (match):**
  - without the `g` flag: an array with the first match plus details (`index`, `input`, `groups`)
  - with the `g` flag: an array of **all** matches
- **Returns (no match):** `null`

```js
"a1b2c3".match(/\d/);    // ["1", index: 1, input: "a1b2c3", groups: undefined]
"a1b2c3".match(/\d/g);   // ["1", "2", "3"]
"abc".match(/\d/);       // null
```

### 12. `matchAll(regexp)`

Returns all matches along with their details, as an iterator.

- **Accepts:** a regular expression (must have the `g` flag)
- **Returns (match):** an iterator of match arrays (use `[...result]` or `for...of`)
- **Returns (no match):** an empty iterator (`[...result]` gives `[]`)

```js
const result = "a1b2".matchAll(/\d/g);
console.log([...result].map(m => m[0]));  // ["1", "2"]

[..."abc".matchAll(/\d/g)];  // []
```

> Throws a `TypeError` if the regex does not have the `g` flag.

---

## Extracting

### 13. `slice(start, end)`

Extracts part of a string from `start` up to (but not including) `end`.

- **Accepts:** `start` (number, can be negative), `end` (optional, can be negative)
- **Returns (match):** the extracted substring
- **Returns (no match):** `""` if `start >= end` or `start` is beyond the string length

```js
"JavaScript".slice(0, 4);    // "Java"
"JavaScript".slice(-6);      // "Script"
"JavaScript".slice(5, 2);    // ""
```

### 14. `substring(start, end)`

Extracts part of a string between two indexes.

- **Accepts:** `start` (number), `end` (optional). Negative values are treated as `0`.
- **Returns (match):** the extracted substring. If `start > end`, the values are swapped.
- **Returns (no match):** `""` if `start` equals `end` or both are beyond the length

```js
"JavaScript".substring(0, 4);   // "Java"
"JavaScript".substring(4, 0);   // "Java"  (swapped)
"JavaScript".substring(2, 2);   // ""
```

### 15. `substr(start, length)` (deprecated)

Extracts a number of characters starting from `start`. Avoid it in new code; use `slice()` instead.

- **Accepts:** `start` (number, can be negative), `length` (optional number of characters)
- **Returns (match):** the extracted substring
- **Returns (no match):** `""` if `length` is `0` or negative, or `start` is beyond the string

```js
"JavaScript".substr(4, 6);    // "Script"
"JavaScript".substr(4, 0);    // ""
```

---

## Modifying / Transforming

### 16. `toUpperCase()`

Converts the string to uppercase.

- **Accepts:** nothing
- **Returns:** a new uppercase string (the same text if it is already uppercase)

```js
"hello".toUpperCase();  // "HELLO"
```

### 17. `toLowerCase()`

Converts the string to lowercase.

- **Accepts:** nothing
- **Returns:** a new lowercase string (the same text if it is already lowercase)

```js
"HELLO".toLowerCase();  // "hello"
```

### 18. `trim()`

Removes whitespace from both ends of the string.

- **Accepts:** nothing
- **Returns (match):** a new string without leading and trailing whitespace
- **Returns (no match):** the same string if there is no whitespace to remove

```js
"  hello  ".trim();   // "hello"
"hello".trim();       // "hello"
```

### 19. `trimStart()`

Removes whitespace from the **start** of the string.

- **Accepts:** nothing
- **Returns (match):** a new string without leading whitespace
- **Returns (no match):** the same string

```js
"  hello  ".trimStart();   // "hello  "
```

### 20. `trimEnd()`

Removes whitespace from the **end** of the string.

- **Accepts:** nothing
- **Returns (match):** a new string without trailing whitespace
- **Returns (no match):** the same string

```js
"  hello  ".trimEnd();   // "  hello"
```

### 21. `padStart(targetLength, padString)`

Adds characters to the **start** until the string reaches the target length.

- **Accepts:** `targetLength` (number), `padString` (optional, default is a space)
- **Returns (match):** a new string padded at the start
- **Returns (no match):** the original string if `targetLength` is less than or equal to the string length

```js
"5".padStart(3, "0");      // "005"
"hello".padStart(3, "0");  // "hello"
```

### 22. `padEnd(targetLength, padString)`

Adds characters to the **end** until the string reaches the target length.

- **Accepts:** `targetLength` (number), `padString` (optional, default is a space)
- **Returns (match):** a new string padded at the end
- **Returns (no match):** the original string if `targetLength` is less than or equal to the string length

```js
"5".padEnd(3, "0");       // "500"
"hello".padEnd(3, "0");   // "hello"
```

### 23. `repeat(count)`

Repeats the string a given number of times.

- **Accepts:** `count` (non-negative number)
- **Returns (match):** the string repeated `count` times
- **Returns (no match):** `""` when `count` is `0`; throws a `RangeError` if `count` is negative or `Infinity`

```js
"ab".repeat(3);   // "ababab"
"ab".repeat(0);   // ""
```

### 24. `replace(pattern, replacement)`

Replaces the **first** match (or all matches if the regex has the `g` flag).

- **Accepts:** `pattern` (string or regex), `replacement` (string or function)
- **Returns (match):** a new string with the replacement made
- **Returns (no match):** the original string, unchanged

```js
"cat cat".replace("cat", "dog");    // "dog cat"
"cat cat".replace(/cat/g, "dog");   // "dog dog"
"cat".replace("bird", "dog");       // "cat"
```

### 25. `replaceAll(pattern, replacement)`

Replaces **all** matches.

- **Accepts:** `pattern` (string or regex with the `g` flag), `replacement` (string or function)
- **Returns (match):** a new string with all matches replaced
- **Returns (no match):** the original string, unchanged

```js
"cat cat".replaceAll("cat", "dog");   // "dog dog"
"cat".replaceAll("bird", "dog");      // "cat"
```

> Throws a `TypeError` if you pass a regex without the `g` flag.

### 26. `concat(...strings)`

Joins one or more strings to the original string.

- **Accepts:** one or more strings (other types are converted to strings)
- **Returns:** a new combined string; with no arguments it returns a copy of the original

```js
"Hello".concat(" ", "World");   // "Hello World"
"Hello".concat();               // "Hello"
```

### 27. `split(separator, limit)`

Splits a string into an array of substrings.

- **Accepts:** `separator` (string or regex), `limit` (optional maximum number of items)
- **Returns (match):** an array of substrings
- **Returns (no match):** an array containing the whole string, `[str]`, if the separator is not found

```js
"a,b,c".split(",");        // ["a", "b", "c"]
"abc".split("");           // ["a", "b", "c"]
"a,b,c".split(",", 2);     // ["a", "b"]
"abc".split(",");          // ["abc"]
```

---

## Comparison

### 28. `localeCompare(compareString)`

Compares two strings in the current locale (dictionary order).

- **Accepts:** `compareString` (string), optional `locales` and `options`
- **Returns:**
  - negative number if the string comes **before** `compareString`
  - `0` if both are **equal**
  - positive number if the string comes **after** `compareString`

```js
"a".localeCompare("b");   // -1 (a comes before b)
"a".localeCompare("a");   // 0
"b".localeCompare("a");   // 1
```

---

## Conversion

### 29. `toString()`

Returns the string value itself.

- **Accepts:** nothing
- **Returns:** the string (a primitive string)

```js
const str = "Hello";
str.toString();   // "Hello"
```

---

## Static Methods

### 30. `String.fromCharCode(...codes)`

Creates a string from UTF-16 character codes. It is called on `String`, not on a string value.

- **Accepts:** one or more numbers (character codes)
- **Returns (match):** a string made from those codes
- **Returns (no match):** `""` if no arguments are given

```js
String.fromCharCode(72, 105);   // "Hi"
String.fromCharCode();          // ""
```

---

## Quick Summary Table

| Method | Returns when found / valid | Returns when not found / invalid |
|---|---|---|
| `charAt()` | character | `""` |
| `charCodeAt()` | char code | `NaN` |
| `at()` | character | `undefined` |
| `indexOf()` | index | `-1` |
| `lastIndexOf()` | index | `-1` |
| `includes()` | `true` | `false` |
| `startsWith()` | `true` | `false` |
| `endsWith()` | `true` | `false` |
| `search()` | index | `-1` |
| `match()` | array | `null` |
| `matchAll()` | iterator | empty iterator |
| `slice()` | substring | `""` |
| `substring()` | substring | `""` |
| `substr()` | substring | `""` |
| `replace()` | new string | original string |
| `replaceAll()` | new string | original string |
| `split()` | array of parts | `[wholeString]` |
| `padStart()` / `padEnd()` | padded string | original string |
| `repeat()` | repeated string | `""` (count `0`) |
| `localeCompare()` | `-1`, `0`, or `1` (sign of result) | not applicable |



# Array Built-in Methods in JavaScript

# Property
1. length

# Adding / Removing Elements
2. push()
3. pop()
4. shift()
5. unshift()
6. splice()

# Accessing / Extracting
7. at()
8. slice()
9. concat()
10. join()
11. flat()
12. flatMap()

# Searching
13. indexOf()
14. lastIndexOf()
15. includes()
16. find()
17. findIndex()
18. findLast()
19. findLastIndex()

# Iteration
20. forEach()
21. map()
22. filter()
23. reduce()
24. reduceRight()
25. some()
26. every()
27. entries()
28. keys()
29. values()

# Sorting / Reordering
30. sort()
31. reverse()
32. toSorted()
33. toReversed()
34. toSpliced()
35. with()

# Filling / Copying
36. fill()
37. copyWithin()

# Conversion
38. toString()
39. toLocaleString()

# Static Methods
40. Array.isArray()
41. Array.from()
42. Array.of()


# Array Built-in Methods in JavaScript

> **Mutating** = changes the original array. **Non-mutating** = returns a new value and leaves the original array unchanged.

---

## Quick Reference: Mutating vs Non-Mutating

| Category | Methods |
|---|---|
| **Mutating (changes original)** | `push`, `pop`, `shift`, `unshift`, `splice`, `sort`, `reverse`, `fill`, `copyWithin` |
| **Non-mutating, returns new array** | `slice`, `concat`, `flat`, `flatMap`, `map`, `filter`, `toSorted`, `toReversed`, `toSpliced`, `with`, `Array.from`, `Array.of` |
| **Non-mutating, returns a value** | `at`, `join`, `indexOf`, `lastIndexOf`, `includes`, `find`, `findIndex`, `findLast`, `findLastIndex`, `reduce`, `reduceRight`, `some`, `every`, `toString`, `toLocaleString`, `Array.isArray` |
| **Non-mutating, returns iterator** | `entries`, `keys`, `values` |
| **Returns nothing (`undefined`)** | `forEach` |

---

## Property

### 1. `length`

Returns the number of elements. It is a property (no parentheses). You can also set it to truncate the array.

- **Mutates original:** Only if you assign to it
- **Returns:** a number

```js
const arr = [1, 2, 3];
arr.length;        // 3
arr.length = 2;    // arr is now [1, 2]
[].length;         // 0
```

---

## Adding / Removing Elements

### 2. `push(...items)`

Adds one or more elements to the **end**.

- **Mutates original:** Yes
- **Returns:** the **new length** of the array

```js
const arr = [1, 2];
arr.push(3, 4);   // returns 4
console.log(arr); // [1, 2, 3, 4]
```

### 3. `pop()`

Removes the **last** element.

- **Mutates original:** Yes
- **Returns (match):** the removed element
- **Returns (empty array):** `undefined`

```js
const arr = [1, 2, 3];
arr.pop();        // 3
console.log(arr); // [1, 2]
[].pop();         // undefined
```

### 4. `shift()`

Removes the **first** element.

- **Mutates original:** Yes
- **Returns (match):** the removed element
- **Returns (empty array):** `undefined`

```js
const arr = [1, 2, 3];
arr.shift();      // 1
console.log(arr); // [2, 3]
[].shift();       // undefined
```

### 5. `unshift(...items)`

Adds one or more elements to the **start**.

- **Mutates original:** Yes
- **Returns:** the **new length** of the array

```js
const arr = [3, 4];
arr.unshift(1, 2);  // returns 4
console.log(arr);   // [1, 2, 3, 4]
```

### 6. `splice(start, deleteCount, ...items)`

Removes, replaces, or inserts elements at any position.

- **Mutates original:** Yes
- **Returns:** an array of the **removed elements** (empty array `[]` if nothing was removed)

```js
const arr = [1, 2, 3, 4, 5];
arr.splice(1, 2);          // returns [2, 3]; arr = [1, 4, 5]
arr.splice(1, 0, "a");     // returns [];     arr = [1, "a", 4, 5]
arr.splice(1, 1, "b");     // returns ["a"];  arr = [1, "b", 4, 5]
```

---

## Accessing / Extracting

### 7. `at(index)`

Returns the element at the index. Supports **negative** indexes.

- **Mutates original:** No
- **Returns (match):** the element
- **Returns (out of range):** `undefined`

```js
const arr = [10, 20, 30];
arr.at(0);     // 10
arr.at(-1);    // 30
arr.at(10);    // undefined
```

### 8. `slice(start, end)`

Copies a portion of the array from `start` up to (not including) `end`.

- **Mutates original:** No
- **Returns:** a **new array** with the selected elements (`[]` if nothing is selected)

```js
const arr = [1, 2, 3, 4, 5];
arr.slice(1, 3);    // [2, 3]
arr.slice(-2);      // [4, 5]
arr.slice(10);      // []
console.log(arr);   // [1, 2, 3, 4, 5] (unchanged)
```

### 9. `concat(...arraysOrValues)`

Joins arrays or values into a new array.

- **Mutates original:** No
- **Returns:** a **new array**

```js
const a = [1, 2];
const b = [3, 4];
a.concat(b, 5);   // [1, 2, 3, 4, 5]
console.log(a);   // [1, 2] (unchanged)
```

### 10. `join(separator)`

Joins all elements into a string. Default separator is a comma.

- **Mutates original:** No
- **Returns:** a **string** (empty string `""` for an empty array)

```js
["a", "b", "c"].join("-");   // "a-b-c"
["a", "b", "c"].join();      // "a,b,c"
[].join("-");                // ""
```

### 11. `flat(depth)`

Flattens nested arrays up to the given depth (default `1`).

- **Mutates original:** No
- **Returns:** a **new flattened array**

```js
[1, [2, [3]]].flat();           // [1, 2, [3]]
[1, [2, [3]]].flat(2);          // [1, 2, 3]
[1, [2, [3, [4]]]].flat(Infinity); // [1, 2, 3, 4]
```

### 12. `flatMap(callback)`

Runs `map()` and then flattens the result by one level.

- **Mutates original:** No
- **Returns:** a **new array**

```js
[1, 2, 3].flatMap(n => [n, n * 2]);   // [1, 2, 2, 4, 3, 6]
```

---

## Searching

### 13. `indexOf(item, fromIndex)`

Returns the first index of the item (uses strict equality `===`).

- **Mutates original:** No
- **Returns (match):** the index
- **Returns (no match):** `-1`

```js
[10, 20, 30].indexOf(20);   // 1
[10, 20, 30].indexOf(99);   // -1
```

### 14. `lastIndexOf(item, fromIndex)`

Returns the last index of the item.

- **Mutates original:** No
- **Returns (match):** the index
- **Returns (no match):** `-1`

```js
[1, 2, 1].lastIndexOf(1);   // 2
[1, 2, 1].lastIndexOf(9);   // -1
```

### 15. `includes(item, fromIndex)`

Checks whether the array contains the item. Unlike `indexOf`, it can find `NaN`.

- **Mutates original:** No
- **Returns (match):** `true`
- **Returns (no match):** `false`

```js
[1, 2, 3].includes(2);       // true
[1, 2, 3].includes(9);       // false
[NaN].includes(NaN);         // true
[NaN].indexOf(NaN);          // -1
```

### 16. `find(callback)`

Returns the **first element** that satisfies the condition.

- **Mutates original:** No
- **Returns (match):** the first matching element
- **Returns (no match):** `undefined`

```js
[5, 12, 8, 20].find(n => n > 10);   // 12
[5, 12, 8, 20].find(n => n > 100);  // undefined
```

### 17. `findIndex(callback)`

Returns the **index** of the first element that satisfies the condition.

- **Mutates original:** No
- **Returns (match):** the index
- **Returns (no match):** `-1`

```js
[5, 12, 8, 20].findIndex(n => n > 10);   // 1
[5, 12, 8, 20].findIndex(n => n > 100);  // -1
```

### 18. `findLast(callback)`

Like `find()`, but searches from the **end**.

- **Mutates original:** No
- **Returns (match):** the last matching element
- **Returns (no match):** `undefined`

```js
[5, 12, 8, 20].findLast(n => n > 10);   // 20
[5, 12, 8, 20].findLast(n => n > 100);  // undefined
```

### 19. `findLastIndex(callback)`

Like `findIndex()`, but searches from the **end**.

- **Mutates original:** No
- **Returns (match):** the index
- **Returns (no match):** `-1`

```js
[5, 12, 8, 20].findLastIndex(n => n > 10);   // 3
[5, 12, 8, 20].findLastIndex(n => n > 100);  // -1
```

---

## Iteration

### 20. `forEach(callback)`

Runs a function once for each element. You cannot stop it with `break`.

- **Mutates original:** No (unless your callback changes it)
- **Returns:** `undefined` (always)

```js
[1, 2, 3].forEach(n => console.log(n));   // 1, 2, 3
const result = [1, 2, 3].forEach(n => n); // result is undefined
```

### 21. `map(callback)`

Transforms every element and returns the results.

- **Mutates original:** No
- **Returns:** a **new array** of the same length

```js
[1, 2, 3].map(n => n * 2);   // [2, 4, 6]
```

### 22. `filter(callback)`

Keeps only the elements that satisfy the condition.

- **Mutates original:** No
- **Returns (match):** a **new array** with matching elements
- **Returns (no match):** an empty array `[]`

```js
[1, 2, 3, 4].filter(n => n % 2 === 0);   // [2, 4]
[1, 2, 3, 4].filter(n => n > 10);        // []
```

### 23. `reduce(callback, initialValue)`

Reduces the array to a **single value** from left to right.

- **Mutates original:** No
- **Returns:** the final accumulated value (the `initialValue` for an empty array)
- **Error:** throws `TypeError` on an empty array with no `initialValue`

```js
[1, 2, 3, 4].reduce((sum, n) => sum + n, 0);   // 10
[].reduce((sum, n) => sum + n, 0);              // 0
```

### 24. `reduceRight(callback, initialValue)`

Same as `reduce()`, but works from **right to left**.

- **Mutates original:** No
- **Returns:** a single value

```js
["a", "b", "c"].reduceRight((acc, s) => acc + s, "");   // "cba"
```

### 25. `some(callback)`

Checks whether **at least one** element satisfies the condition.

- **Mutates original:** No
- **Returns (match):** `true`
- **Returns (no match):** `false` (also `false` for an empty array)

```js
[1, 2, 3].some(n => n > 2);    // true
[1, 2, 3].some(n => n > 10);   // false
```

### 26. `every(callback)`

Checks whether **all** elements satisfy the condition.

- **Mutates original:** No
- **Returns (all match):** `true` (also `true` for an empty array)
- **Returns (any fails):** `false`

```js
[2, 4, 6].every(n => n % 2 === 0);   // true
[2, 3, 6].every(n => n % 2 === 0);   // false
```

### 27. `entries()`

Returns an iterator of `[index, value]` pairs.

- **Mutates original:** No
- **Returns:** an **iterator** (use `for...of` or spread)

```js
const arr = ["a", "b"];
[...arr.entries()];   // [[0, "a"], [1, "b"]]
```

### 28. `keys()`

Returns an iterator of the indexes.

- **Mutates original:** No
- **Returns:** an **iterator**

```js
[..."ab"].keys();            // iterator
[...["a", "b"].keys()];      // [0, 1]
```

### 29. `values()`

Returns an iterator of the values.

- **Mutates original:** No
- **Returns:** an **iterator**

```js
[...["a", "b"].values()];    // ["a", "b"]
```

---

## Sorting / Reordering

### 30. `sort(compareFn)`

Sorts the array **in place**. Without a compare function it sorts as **strings** (so numbers sort incorrectly).

- **Mutates original:** Yes
- **Returns:** the **same array** (reference to the original, sorted)

```js
[10, 9, 1].sort();                 // [1, 10, 9]  (string order)
[10, 9, 1].sort((a, b) => a - b);  // [1, 9, 10]  (ascending)
[10, 9, 1].sort((a, b) => b - a);  // [10, 9, 1]  (descending)
```

### 31. `reverse()`

Reverses the array **in place**.

- **Mutates original:** Yes
- **Returns:** the **same array** (reversed)

```js
const arr = [1, 2, 3];
arr.reverse();     // [3, 2, 1]
console.log(arr);  // [3, 2, 1]
```

### 32. `toSorted(compareFn)` (ES2023)

Same as `sort()`, but returns a **new** sorted array.

- **Mutates original:** No
- **Returns:** a **new array**

```js
const arr = [3, 1, 2];
arr.toSorted((a, b) => a - b);   // [1, 2, 3]
console.log(arr);                // [3, 1, 2] (unchanged)
```

### 33. `toReversed()` (ES2023)

Same as `reverse()`, but returns a **new** reversed array.

- **Mutates original:** No
- **Returns:** a **new array**

```js
const arr = [1, 2, 3];
arr.toReversed();   // [3, 2, 1]
console.log(arr);   // [1, 2, 3] (unchanged)
```

### 34. `toSpliced(start, deleteCount, ...items)` (ES2023)

Same as `splice()`, but returns a **new** array and leaves the original unchanged.

- **Mutates original:** No
- **Returns:** a **new array** with the changes applied

```js
const arr = [1, 2, 3, 4];
arr.toSpliced(1, 2, "x");   // [1, "x", 4]
console.log(arr);           // [1, 2, 3, 4] (unchanged)
```

### 35. `with(index, value)` (ES2023)

Returns a new array with the element at the index replaced.

- **Mutates original:** No
- **Returns (valid index):** a **new array**
- **Returns (invalid index):** throws `RangeError`

```js
const arr = [1, 2, 3];
arr.with(1, 99);    // [1, 99, 3]
console.log(arr);   // [1, 2, 3] (unchanged)
arr.with(10, 99);   // RangeError
```

---

## Filling / Copying

### 36. `fill(value, start, end)`

Fills elements with a static value.

- **Mutates original:** Yes
- **Returns:** the **same array**

```js
[1, 2, 3, 4].fill(0);        // [0, 0, 0, 0]
[1, 2, 3, 4].fill(0, 1, 3);  // [1, 0, 0, 4]
new Array(3).fill("x");      // ["x", "x", "x"]
```

### 37. `copyWithin(target, start, end)`

Copies part of the array to another position **within the same array**.

- **Mutates original:** Yes
- **Returns:** the **same array**

```js
[1, 2, 3, 4, 5].copyWithin(0, 3);   // [4, 5, 3, 4, 5]
```

---

## Conversion

### 38. `toString()`

Converts the array to a comma-separated string.

- **Mutates original:** No
- **Returns:** a **string**

```js
[1, 2, 3].toString();   // "1,2,3"
[].toString();          // ""
```

### 39. `toLocaleString()`

Converts the array to a string using locale-specific formatting for each element.

- **Mutates original:** No
- **Returns:** a **string**

```js
[1234.5, new Date(0)].toLocaleString("en-US");
// "1,234.5,1/1/1970, 12:00:00 AM" (depends on locale and timezone)
```

---

## Static Methods

### 40. `Array.isArray(value)`

Checks whether a value is an array.

- **Mutates original:** Not applicable
- **Returns (array):** `true`
- **Returns (not array):** `false`

```js
Array.isArray([1, 2]);    // true
Array.isArray("hello");   // false
Array.isArray({});        // false
```

### 41. `Array.from(iterable, mapFn)`

Creates a **new array** from an iterable or array-like object (string, Set, Map, `arguments`, etc.).

- **Mutates original:** No
- **Returns:** a **new array**

```js
Array.from("abc");                       // ["a", "b", "c"]
Array.from(new Set([1, 1, 2]));          // [1, 2]
Array.from({ length: 3 }, (_, i) => i);  // [0, 1, 2]
```

### 42. `Array.of(...items)`

Creates a **new array** from the given arguments.

- **Mutates original:** Not applicable
- **Returns:** a **new array**

```js
Array.of(3);        // [3]
Array(3);           // [ <3 empty items> ]  (different!)
Array.of(1, 2, 3);  // [1, 2, 3]
```

---

## Summary Table: Return Values

| Method | Returns | Mutates? | If match / success | If no match / fail |
|---|---|---|---|---|
| `push()` | new length | Yes | length | n/a |
| `pop()` | removed element | Yes | element | `undefined` |
| `shift()` | removed element | Yes | element | `undefined` |
| `unshift()` | new length | Yes | length | n/a |
| `splice()` | removed elements array | Yes | `[removed]` | `[]` |
| `at()` | element | No | element | `undefined` |
| `slice()` | new array | No | `[items]` | `[]` |
| `concat()` | new array | No | combined array | n/a |
| `join()` | string | No | joined string | `""` |
| `flat()` | new array | No | flattened array | n/a |
| `flatMap()` | new array | No | flattened array | `[]` |
| `indexOf()` | number | No | index | `-1` |
| `lastIndexOf()` | number | No | index | `-1` |
| `includes()` | boolean | No | `true` | `false` |
| `find()` | element | No | element | `undefined` |
| `findIndex()` | number | No | index | `-1` |
| `findLast()` | element | No | element | `undefined` |
| `findLastIndex()` | number | No | index | `-1` |
| `forEach()` | `undefined` | No | `undefined` | `undefined` |
| `map()` | new array | No | transformed array | `[]` (empty array) |
| `filter()` | new array | No | matching items | `[]` |
| `reduce()` | single value | No | final value | `initialValue` (empty array) |
| `some()` | boolean | No | `true` | `false` |
| `every()` | boolean | No | `true` | `false` |
| `sort()` | same array | Yes | sorted array | n/a |
| `reverse()` | same array | Yes | reversed array | n/a |
| `toSorted()` | new array | No | sorted array | n/a |
| `toReversed()` | new array | No | reversed array | n/a |
| `toSpliced()` | new array | No | changed copy | n/a |
| `with()` | new array | No | changed copy | `RangeError` |
| `fill()` | same array | Yes | filled array | n/a |
| `copyWithin()` | same array | Yes | modified array | n/a |
| `toString()` | string | No | string | `""` |
| `Array.isArray()` | boolean | n/a | `true` | `false` |
| `Array.from()` | new array | No | new array | `[]` |
| `Array.of()` | new array | n/a | new array | `[]` |