# Gaba Programming Language Tutorial

Welcome to Gaba!

This tutorial teaches every feature currently implemented.

---

# Hello World

```gaba
say("Hello World")
```

---

# Variables

```gaba
let name = "Divansh"

let age = 18
```

---

# Printing Variables

```gaba
say(name)

say(age)
```

---

# Arithmetic

```gaba
say(10+5)

say(20-3)

say(4*5)

say(40/8)
```

---

# Parentheses

```gaba
say((5+5)*3)
```

---

# Comparisons

```gaba
say(5==5)

say(10>5)

say(3<=7)
```

---

# Input

```gaba
let name = ask("Name: ")

say(name)
```

---

# Assignment

```gaba
let score = 10

score = score + 5

say(score)
```

---

# if

```gaba
let age = 20

if age>=18{

    say("Adult")

}
```

---

# if else

```gaba
let age = 12

if age>=18{

    say("Adult")

}
else{

    say("Minor")

}
```

---

# while

```gaba
let i = 1

while i<=5{

    say(i)

    i=i+1

}
```

---

# Functions

```gaba
fun greet(name){

    say("Hello")

    say(name)

}

greet("Divansh")
```

---

# Returning Values

```gaba
fun add(a,b){

    give a+b

}

say(add(5,10))
```

---

# Example Calculator

```gaba
fun add(a,b){

    give a+b

}

let x = ask("First Number: ")

let y = ask("Second Number: ")

say(add(x,y))
```

> **Note:** Currently `ask()` returns strings. Automatic number conversion is not implemented yet, so arithmetic with user input may not behave as expected.

---

# Current Language Limitations

The following features are **not implemented yet**:

- Lists
- Arrays
- Dictionaries
- for loops
- break
- continue
- switch
- import
- modules
- objects
- classes
- inheritance
- interfaces
- enums
- exceptions
- file handling
- networking
- multithreading
- package manager
- compiler

---

# Common Errors

## Undefined variable

```gaba
say(name)
```

Error

```
Undefined variable 'name'
```

Solution

Declare it first.

```gaba
let name = "Gaba"
```

---

## Undefined function

```gaba
hello()
```

Error

```
Undefined function 'hello'
```

Solution

Declare the function before calling it.

---

## Wrong number of arguments

```gaba
fun add(a,b){

    give a+b

}

add(5)
```

Error

```
Function 'add' expects 2 arguments.
```

---

## Infinite while loop

```gaba
let i = 1

while i<10{

    say(i)

}
```

This never ends.

Always update the loop variable.

```gaba
i = i + 1
```

---

# Best Practices

- Use meaningful variable names.
- Keep functions small.
- Prefer returning values with `give` instead of printing from inside functions when possible.
- Test new features in small `.gaba` files before using them in larger programs.
- Keep one regression test file that exercises all language features after every change.

---

# Current Version

Gaba v0.0.3