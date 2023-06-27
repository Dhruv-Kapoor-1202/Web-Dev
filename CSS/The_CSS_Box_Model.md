# Box Model: Width and Height

The *width* CSS property sets an element's width. By default, it sets the width of the **content area**, (but it *box-sizing* is set to *border-box*, it sets the width of the border area.)

Same think goes for height.  
  
Width and Height control the actual content area.

# Box Model: Border and Border-Radius

# Box Model: Padding

Individual Properties:
- padding-left
- padding-right
- padding-bottom
- padding-top

Shorthand Property  
Sets all four sides at once!  
  
# Box Model: Margin

Similar to padding, just works outside the border.  

# The Display Property 

(Our first encounter)

|Inline|Block|Inline-Block|
|-|-|-|
|Width & height are ignored. Margin & padding push elements away horizontally but not vertically.|Block elements break the flow of a document. Width, height, Margin, & Padding are respected.|Behaved like an inline element except Width, Height, Margin, & Padding are respected.| 

# CSS Units

Relative 
- EM
- REM
- VH
- VW
- %
- And More
  
Absolute 
- PX
- PT
- CM
- IN
- MM

## Percentages

**Percentages are alwasy relative to some other value**  
Sometime, it's a value from the parent other times it's a vlue from the element itself.  
`width: 50%` - half the width of the parent  
`line-height: 50%` - half the font-size of the element itself

## EM

**EM's are Relative units**  
With font-size, 1em equals the font-size of the parent. 2em's is twice the font-size of the parent, etc.  
With other properties, 1em is equal to the computed font-size of the element itself.

## REM 

**Root EMs**  
Relative to the **root html element's** font size. Often easier to work with.  
If the root font-size is 20px, 1em is always 20px, 2rem is always 40px, etc.  
