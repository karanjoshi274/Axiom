# 🧠 Axiom

**Axiom** is a mini programming language built entirely from scratch using **JavaScript**, designed to mimic core features found in real-world languages. This project explores the **fundamentals of language design** by implementing concepts like **closures**, **variable scoping**, **function execution**, and **custom evaluation logic**.

> 🛠 The goal of Axiom is not performance or production-readiness, but rather to deepen understanding of how programming languages work under the hood.

---

## ⚡ Demo

Check out a recursive `fizzbuzz` function implemented in Axiom:

```js
fn fizzbuzz(n) {
    if (n % 15 == 0) {
        print("FizzBuzz")
    } elseif (n % 3 == 0) {
        print("Fizz")
    } elseif (n % 5 == 0) {
        print("Buzz")
    } else {
        print(n)
    }

    if (n < 100) {
        fizzbuzz(n + 1)
    }
}

fizzbuzz(1)
```
⚙️ How to Use
Although NPM is not required to run Axiom, it is needed if you want to run the test suite.

✅ Prerequisite (for testing)
Make sure you have Node.js and NPM installed.
To install NPM (if not already installed):

```bash
npm install npm@latest -g
```
🚀 Getting Started
Clone the Repository

```bash
git clone https://github.com/karanjoshi274/Axiom.git
cd Axiom
```
Install Dependencies (for testing only)

```bash
npm install
```
Run Axiom Code
Navigate to the src directory and modify the test.txt file with your Axiom code.

Then run:

```bash
node main.js
```
You’ll see the interpreted output in the terminal.

🧪 Running Tests
Run the full test suite:

```bash
npm test
```
To run a specific test file:

```bash
npm test evaluator.test.js
```
📜 Supported Syntax
✅ Value Types
```js
12                // NumericLiteral
"Hello" or 'Hi'   // StringLiteral
true, false       // BooleanLiteral
null              // NullLiteral
{one: 1}          // ObjectLiteral
```
🆔 Identifiers
```js
foo
```
➕ Binary Operators
```js
+  -  *  /  %
```
🔁 Comparison Operators
```js
==  !=  <  <=  >  >=
```
🔗 Logical Operators
```js
&&  ||
```
🔂 Unary Operators
```js
!value

// No '-' unary operator yet. Use:
-1 * value
```
📄 Conditional Statements
```js
if (condition1) {
    // block
} elseif (condition2) {
    // block
} else {
    // block
}
```
🧠 Function Declaration
No return keyword — the last evaluated statement is returned automatically.

```js
fn add(x, y) {
    x + y
}
```
📞 Function Call
```js

add(2, 3)
```
🧾 Variable Declarations
```js

const foo = 42
let bar = 12
bar = 100

let something;  // uninitialized variable
```
🌐 Native Functions
print() is currently the only built-in native function.

Works just like console.log() in JavaScript.

```js

print("Hello, Axiom!")
```
### 📬 Contact
For suggestions, improvements, or feedback, feel free to open an issue or contribute on GitHub:
👉 https://github.com/karanjoshi274/Axiom

"Building a language from scratch teaches you more about programming than using one ever will."
