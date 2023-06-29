# Why JavaScript is Awesome

# Primitives & The Console

Steps:  
1. Learn JS on its own. No HTML/CSS
2. Use JS to manipulate HTML/CSS  
   
## Primitive Types 

The basic building blocks:  
- Number
- String
- Boolean
- Null
- Undefined

Note: Technically there are two others: Symbol and BigInt.  
  
## Running Cde in the Console

R E P L  
R: Read  
E: Evalute  
P: Print  
L: Loop  
  
# JavaScript Numbers

- JS has **one** number type
- Positive numbers
- Negative numbers
- Whole numbers (integers)
- Decimal numbers
  
Built in math operators  
- +
- -
- /
- *
- %
- **

# WTF is NaN

Not A Number  

NaN is a numeric value that represents something that is ...not a number.  
  
```javascript
0/0 //NaN
1 + NaN //NaN
```

# Variables & Let

## Variables

Variables are like labels for values  
  
We can store a value and give it a name so that we can:
- Refer back to it later
- Use that value to do ...stuff
- Or change it later on

Basic Syntax

```javascript
// let someName = value;
let year = 1985;
```

# Updating Variables

score = score + 5;   
score += 5;
  
score++;  
score--;  
  
# Increment Operator Explanation: i++ vs ++i

i++: postfix increment operator  
It first returns the current value of i and then increments it by one.  
  
++i: prefix increment operator
It increments the value of the variable by one first and then returns the incremented value.

# Const & Var

## Const

Const works just like let, except you CANNOT change the value

## Var

The old variable keyword.  
Before let and const, var was the only way of declaring variables. These days, there isn't really a reason to use it.  
  
# Booleans

Two possible options: true or false

## **Variables can change types**

```javascript
let numPuppies = 23;
numPuppies = false;
numPuppies = 100;
```

# Variable Naming and Conventions