# Decision Making With Cod

Boolean Logic

# Comparison Operators

```Javascript
>  //  greator than
<  //  less than
>=  // greator than or equal to 
<=  // less than or equal to
==  // equality
!=  // not equal
=== // strict equality
!== // strict non-equality
```

Returns a boolean value

# Equality: Triple Vs. Double Equals

## == (double equals)
- Checks for equality of value, but not equality of type.
- It coerces both values to the same type and then compares them.
- This can lead to some unexpected results!

```Javascript
1 == 1 ;  // true
1 == '1'; // true
0 == '';  // true
'b' == 'c'; //false
0 == false;  //true
null == undefined;  //true
```

## triple equals

```Javascript
5 === 5;  // true
1 === 2;  // false
2 === '2'; // false
false === 0;  //false

//same applies for != and !==
10 != '10';   // false
10 !== '10';  // true
```

Checks for equality of value and type

# Console, Alert, & Prompt

- console.log()
  - prints arguments to the console
- alert
  - also prints out argument but not in console. It pops out an alert
- prompt
  - similar to alert but it asks for user input.
- parseInt("97");
  - gives out the integer value of the string

# Running JavaScript From A Script

- make a javascript file with the extension of .js.
- In the index.html, using the script element and its src attribute, connect the js file to the html file.

# If Statements

```Javascript
if (condition) {
    //code that runs if the condition is true.
}
```

# Else-if

If not the first thing, maybe this other thing??

```Javascript
if (condition 1) {
    //code that runs if the condition is true. 
}
else if (condition 2) {
    //code that runs if the first condition is false and the second condition is true.
}
```

# Else