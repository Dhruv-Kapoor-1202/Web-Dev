# What on Earth is Flexbox?

## What is it? 
Flexbox is a one-dimensional layout method for laying out items in rows or columns.

## It's new(ish)
Flexbox is a recent addition to CSS, included to address common layout frustrations.

## Why 'FLEX'?
Flexbox allows us to distribute space dynamically across elements of an unknown size, hence the term 'flex'.

# Flex-Direction

```CSS
display: flex;
```

main axis: left to right
cross axis: top to bottom
  
flex-direction can help us change between these two axis. By default it is row.

flex-direction:  
- row
- row-reverse
- column
- column-reverse

# Justify-content

It determines how the content is distributed across the **main axis**.  
  
Defualt flex-start.  
If the main axis is from left to right, then flex start is also left to right. If it is right to left, then the flex-start is also right to left.  

justify-content:  
- flex-start
- flex-end
- center
- space-between
- space-around
- space-evenly

# Flex-wrap

```css
flex-wrap: wrap;
```
flex-wrap:  
- wrap
- no-wrap
- wrap-reverse

# Align-items

Distributes space along the **cross axis**.  
Default - flex-start  
  
align-items:  
- flex-start
- flex-end
- center
- baseline ---- if there is text in the elements, its going to use the baseline of the text to align the items. Usually it just uses the element itself.

# Align-content and align-self

## Align Content

```css
align-content: space-between;
```
   
We use this to control or distribute space along the **cross axis** but only when we have multiple rows or columns depending on the layout.
  
align-content:  
- space-between
- flex-start
- flex-end
- center
  
It only works with wrap or wrap-reverse.  
  
# Align Self

Very similar to align-items, except its a property we add to a single element or to individual items in a container. 

# Flex-Basis, Grow or Shrink

## Flex-Basis
Defines the initial size on element before additional space is distributed.
  
It works along the main axis. If the width given is 200px, and flex-basis is 400px, the elements will be 400px, only if the main axis is horizontal. But if it is virtical, the width will be 200px but the height will 400px.

## Flex-Grow
Controls the amoutn of available space an elemtn should take up. Accepts a unit-less number value.

## Flex-Shrink
If items are larger than the container, they shrink according to flex-shrink.

# Flex Shorthand

- keyword values
  - auto
  - initial
  - none
- **one value**
  - unitless: flex-grow
  - width/height: flex-basis
- **two values**
  - flex-grow | flex-basis
  - flex-grow | flex-shrink
- **three values**
  - flex-grow | flex-shrink | flex-basis
- Global values
  - inherit
  - initial
  - unset

# Responsive Design And Media Queries Intro

## The Problem
As mobile devices and tablets became widely available, developers had a problem... how do we create websites that look good on all screen sizes?

## One Approch
Early on it was common to create separate stylesheets for different devices, or even completely different websites for each size.

## Enter Responsive
These days, we typically create ONE website and stylesheet that is able to respond to different device sizes and features.

## Media Queries
Media queries allow us to modufy our styles depending on particular parameters like screen width or device type.

# The Power of Media Queries

# Reset CSS

```css
/* http://meyerweb.com/eric/tools/css/reset/ 
   v2.0 | 20110126
   License: none (public domain)
*/

html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed, 
figure, figcaption, footer, header, hgroup, 
menu, nav, output, ruby, section, summary,
time, mark, audio, video {
	margin: 0;
	padding: 0;
	border: 0;
	font-size: 100%;
	font: inherit;
	vertical-align: baseline;
}
/* HTML5 display-role reset for older browsers */
article, aside, details, figcaption, figure, 
footer, header, hgroup, menu, nav, section {
	display: block;
}
body {
	line-height: 1;
}
ol, ul {
	list-style: none;
}
blockquote, q {
	quotes: none;
}
blockquote:before, blockquote:after,
q:before, q:after {
	content: '';
	content: none;
}
table {
	border-collapse: collapse;
	border-spacing: 0;
}
```