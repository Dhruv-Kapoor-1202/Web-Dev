# Introducing HTML Tables

What are Tables?  
> Tables are structured sets f data, made up of rows and columns. They can be a great way of diplaying data clearly.

# Tables: TR, TD and TH Element

```HTML
<table>
    <caption></caption>
    <tr>
        <th></th>
        <th></th>
    </tr>
    <tr>
        <td></td>
        <td></td>
    </tr>
</table>
```

# Tables: Thead, Tbody and Tfoot Elements

```HTML
<table>
    <caption></caption>
    <thead>
        <tr>
            <th></th>
            <th></th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>
```

# Tables: Colspan and Rowspan

```
<table>
    <caption></caption>
    <thead>
        <tr>
            <th rowspan="2">1</th>
            <th colspam="2">2</th>
            <th rowspan="2">3</th>
        </tr>
        <tr>
            <th>2 A</th>
            <th>2 B</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td></td>
            <td></td>
            <td></td>
            <td></td>
        </tr>
    </tbody>
</table>
```

# Forms

## Creating Forms
- The `<form>` element itself is a shell or container that doesn't have any visual impact.
- We then fill the form with a collection of inputs, checkboxes, buttons, etc.
  
### `<form>`

- The form element "represents a document section containing interactive controls for submitting information."
- The __action__ attribute specifies WHERE the form data should be sent.
- The __method__ attribute specifies which HTTP method should be used.

```HTML
<form action="" method="">
</form>
```

### `<input>`

- The input element is usd to create a variety of different form controls.
- We have 20+ possible tpes of inputs, ranging from date pickers to checkboxes.
- The __type__ attribute is where the magic happens. Changing __type__ dramaically alter the input's behaviour and appearance.

```HTML
<form>
    <input type="text" placeholder="Username">
    <input type="password" placeholder="Password">
    <input type="color">
    <input type="number" placeholder="Enter a number">
    <input type="time">
</form>
```

### `<label>`

```HTML
<form>
    <p>
        <label for="username">Enter Username:</label>
        <input type="text" placeholder="Username" id="username">
    </p>
    <p>
        <label for="password">Enter Password:</label>
        <input type="password" placeholder="Password" id="password">
    </p>
    <p>
        <label for="color">Enter a color:</label>
        <input type="color" id="color">
    </p>
    <!-- The other way -->
    <p>
        <label>
            Enter a number:
            <input type="number" placeholder="Enter a number">
        </label>
    </p>
</form>
```

### `<button>`

```HTML
<form action="/tacos">
    <p>
        <label for="username">Enter Username:</label>
        <input type="text" placeholder="Username" id="username">
    </p>
    <p>
        <label for="password">Enter Password:</label>
        <input type="password" placeholder="Password" id="password">
    </p>
    <p>
        <label for="color">Enter a color:</label>
        <input type="color" id="color">
    </p>
    <!-- The other way -->
    <p>
        <label>
            Enter a number:
            <input type="number" placeholder="Enter a number">
        </label>
    </p>

    <!-- By default if it is inside the form, it submits that form. -->
    <button>Submit</button>


    <button type="button">button</button>
    <button type="submit">button</button>
    <input type="submit" value="Click me!!!">
    
</form>
<!-- Doesnt submit the form -->
<button>Outside form</button>
```

### The __name__ attribute

```HTML
<form action="/tacos">

    <!-- file:///tacos?username=chickenman -->

    <p>
        <label for="username">Enter Username:</label>
        <input type="text" placeholder="Username" id="username" name="username">
    </p>
    <p>
        <label for="password">Enter Password:</label>
        <input type="password" placeholder="Password" id="password" name="password">
    </p>
    <p>
        <label for="color">Enter a color:</label>
        <input type="color" id="color" name="color">
    </p>
    <button>Submit</button>
</form>
```

### "Hijacking" Google & Reddit's Search

```HTML
<form action="https://www.reddit.com/search">
    <input type="text" name="q">
    <button>Search Reddit</button>
</form>

<form action="https://www.google.com/search">
    <input type="text" name="q">
    <button>Search Google</button>
</form>

<form action="https://www.youtube.com/results">
    <input type="text" name="search_query">
</form>
```

## HTML5 Form Validations

### HTML attribute: required

```HTML
<form action="/dummy">
    <label for="first">Enter First Name:</label>
    <input type="text" name="first" id="first" required>
    <button>Submit</button>
</form>
```

### HTML attribute: minlength, maxlength

```HTML
<form action="/dummy">
    <label for="first">Enter First Name:</label>
    <input type="text" name="first" id="first" required>

    <label for="username">Username</label>
    <input type="text" id="username" name="username" minlength="5" maxlength="20" required>
    <button>Submit</button>
</form>
```

### HTML attribute: pattern

 