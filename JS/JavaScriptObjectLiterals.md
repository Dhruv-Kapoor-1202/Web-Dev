# Introducing Object Literals

- Objects are collections of *properties*
- Properties are a key-value pair
- Rather tan accessing data using an index, we use custom keys.

# Creating Object Literals

```javascript
const person = {
  firstName: 'Mick',
  lastName: 'Jagger'
}

const person = {
  name: 'Mick',
  score: 192,
  isguilded: true,
  stuff: [1, 2, 3, 4],
  otherStuff: {
    key: "value"
  }
}
```

# Accessing data out of Objects

```javascript
person["lastName"]

person.lastName;
```
  
**Valid Keys**  
All keys are converted to strings (Except for Symbols)   
  
# Modifying Objects

# Nesting Arrays and Objects

