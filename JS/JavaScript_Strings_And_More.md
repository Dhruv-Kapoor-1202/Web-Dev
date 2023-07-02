# Introducing Strings

"String of Characters"  
Strings are another primitive type in JavaScript. They represent text, and must be wrappped in quotes.  
  
# Indices & Lenght

Each character has a corresponding index (a positional number)  
  
# String Methods

Methods are built-in actions we can perfom with individual strings.  
  
They help us do things like:
- Searching within a string
- Replacing part of a string 
- Changing the casing of a string

```javascript
"lol".length; //Property
"lol".toLowerCase(); //Method
```

Non destructive method: The original variable is not changed. It makes a new copy.

# String Methods With Arguments

Some methods accept **arguments** that modify their behaviour. Think of them as input that we can pass in. We pass thses arguments inside of the parentheses.  
  
# String Template Literals

Template literals are strings that allow embedded expressions, which will be evaluated and then turned into a resulting string.

```javascript
`I counted ${3 + 4} sheep`; // I counted 7 sheep"
```  
  
**We use back-ticks not single quotes**  
`I am a template literal`  
*Above the Tab

# Undefined and Null

- Null
  - "Intentional absence of any value"
  - Must be assigned
- Undefined
  - Variables that do not have an assigned value are undefined


# Random Numbers & The Math Object

## Math Object  
Contains properties and methods for mathematical constants and functions.

```Javascript
Math.PI;
Math.round(4.9);
Math.pow(2, 5);
Math.floor(3.9999);
```

## Random Numbers
Math.random() gives us a random decimal between 0 and 1 (non-inclusive)  
```Javascript
Math.random(); // between 0 and 1
```
No randomInt, we have to calculate for the custom ranges.  
  
```Javascript
Math.floor(Math.random() * 10) + 1; // 1 to 10
```

