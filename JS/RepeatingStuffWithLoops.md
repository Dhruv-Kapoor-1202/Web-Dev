# Intro to For Loops

- Loops allow us to repeat code
- There are multiple types of loops: 
  - for loop
  - while loop
  - for ...of loop
  - for ...in loop
  
For Loop Syntax: 
```
for (
  [initialExpression];
  [condition];
  [incrementExpression]
) 
```

# The Perils of Infinite Loops

# Looping over Arrays

```javascript
const animals  = ['lion', 'tigers', 'bears'];

for (let i = 0; i < animals.length; i++) {
  console.log(i, animals[i]);
}
```

# Nested Loops

# Another Loop: The While Loop

```javascript
let count = 0; 
while (count < 10) {
  console.log(count);
  count++;
}
```

# The Break Keyword

