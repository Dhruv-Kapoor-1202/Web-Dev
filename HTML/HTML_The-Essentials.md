# Intro to HTML

HTML: Hyper Text Markup Language

Grading a test or a poem, checking the ssppeelllliinnggss



# Mozilla Developer Network

Resources for developers, by developers.  



# Headings

Dont use them according to the size.  
Use them according to what the number represents  
  
Dont use an h3 without an h1 and h2 first.



# HTML Boilerplate

```HTML
<!DOCTYPE html>
<html>
    <head>
        <title></title>
    </head>
    <body>
    </body>
</html>
```



# List Element

Two types of lists:
- Ordered list `<ol>`
- Unordered list `<ul>`
  
Other than `<templates>` and `<script>` tags, **only `<li>` tags are permitted** inside an unordered list or an ordered list.

```HTML
<ul>
    <li></li>
    <li>
        <b>bold text</b>
    </li>
    <li></li>
</ul>

<ol>
    <li></li>
    <li></li>
    <li></li>
</ol>
```
  
The list can only have li tag as a direct children but the li tag can have any other tags inside them.  
  
Lists can have lists inside them - **Nested lists.**  
  

# Achor Tags

With its `href` **attribute** (Hypertext Reference), creates a hyperlink to webpages, files, email addresses, locations in the same page, or anything else a URL can address. Content within each `<a>` shoudl indicate the link's destination.  
  

# Images

Does not have a closing tag.  

```HTML
<img src="" alt="">
```  
  
name of the image + extension + the folder in which the image is located.

# Comments
  
```HTML
<!-- ahhhhhh a comment -->
```


  
