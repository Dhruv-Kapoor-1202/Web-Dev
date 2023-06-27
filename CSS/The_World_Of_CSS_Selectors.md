# Universal and Elemental Selectors

## Universal Selector

```CSS
* {
    color: black;
}
```

## Element Selector

```CSS
button {
    color: magenta;
}
```

## Selector List 

```CSS 
h1, h2 {
    color: magenta;
}
```

# The ID Selector

Select the element with id of 'logout'

```CSS
#logout {
    color: orange;
    height: 200px;
}
```

# The Class Selector

Select elements with class of 'complete'

```CSS 
.complete {
    color: green;
}
```

# Descendant Selector

Select all `<a>`'s that are nested inside an `<li>`

```CSS
li a {
    color: teal;
}
```

# Adjacent Selector 

Select only the paragraphs that are immediately preceded by an `<h1>`  

The **+** sign is called the **Adjacent Combinator**.
  
```CSS
h1 + p {
    color: red;
}
```

# Direct Child Selector/Combinator

Select only the `<li>`'s that are direct children of a `<div>` element

```CSS 
div > li {
    color: white;
}
```

# The Attribute Selector

Select all input elements where the type attribute is sat to "text"

```CSS 
input[type="text"] {
    width: 300px;
    color: yellow;
}
```

# Pseudo Classes

Keyword added to a selector that specifies a special state of the selected element(s)
- :active
- :checked
- :first
- :first-child
- :hover
- :not()
- :nth-child()
- :nth-of-type()

# Pseudo Element 

Keyword added to a selector that lets you style a particular part of selected element(s)

- ::after
- ::before
- ::first-letter
- ::first-line
- ::selection

# The Cascade 

The order you styles are declared in and linked to matters!

```CSS
h1 {
    color: red;
}
h1 {
    color: purple;
}
```
**PURPLE WINS**

# Specificity

**Q.** What happens when conflicting styles target the same element?  
  
  
**Specificity**  
Specificity is how the brow ser decides which rules to apply when multiple rules could appluu to the same element.  
  
It is a measure of how specific a given selector is. The more specific selector "wins".  
  
**ID > Class > Element**  
  
```CSS
nav a.active {
    color: orange;
}
```

| 0 | 1 | 2 |
|:-:|:-:|:-:|
|ID Selectors|Class, Attribute, & Pseudo-clas Selectors|Element and Pseudo-element Selectors|
  
# Inline Styles

**Specificity:  
 Inline Styles > ID selectors > Class, Attribute, & Pseudo-clas Selectors > Element and Pseudo-element Selectors**

# CSS Inheritance

