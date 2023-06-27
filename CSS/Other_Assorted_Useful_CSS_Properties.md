# Opacity And The Alpha Channel

**`background-color: rgba(255, 255, 255, 1);`**  
**`background-color: #00ccaa00 to 00ccaaff;`**  
Alpha: 0 to 1   
Alpha is clubbed along with the rgb and it is genrally for that element only - background or whatever.  
  
Opacity: 0 to 1  
Opacity affects the entire element or any decendants of the element it is applied to.

# The Position Property

The *position* **CSS** property sets how an element is positioned in a document. The *top*, *right*, *bottom*, and *left* properties determine the final location of positioned elements.  
  
- **static**
  - The elemnt is positoned according to the normal flo od the document. The *top*, *right*, *bottom*, *left*, and *z-index* properties have no-effect. This is the default value.
- **relative**
  - The element is positioned according to the normal flow of the document, and then offset *relative to itself* based on the values of *top*, *right*, *bottom*, and *left*. The offset does not affect the position of any other elements; thus, the sace given for the element in the page layout is the same as if position were *static*.  
  - This value creates a new **Stacking context** when the value of *z-index* is not *auto*.
- **absolute**
  - The element is removed from the normanl document flow, and no space is created for the element in the page layout. It is positioned relative to its closest positioned ancestor, if any; otherwise, it is placed relative to the initial **containing block**. Its final position is determined by the values of *top*, *right*, *bottom*, and *left*.
  - This value creates a new **Stacking context** when the value of z-index is not **auto**. The margins of absolutly positioned boxes do not collapse with other margins.
- **fixed**
  - The element is removed from the normal document flow, and no space is created for the element in the page layout. It is positioned relative to the initial **containing block** established by the **viewport**, excet when one of its ancestors has a *transform*, *perspective*, or *filter* property set to something other than **none**, in which case that ancestor behaves as the containing block. Its final positionis determined by the valuse of *top*, *right*, *bottom*, and *left*.
  - This value always creates a **stacking content**. In printed documents, the element is placed in the same postion on every page.
- **sticky**
  - The element is positioned according to the normal flow of the document, and then offset relative to its *nearest scrolling ancestor* and **containing block** (nearest block level ancestor), include table-related elements, based on the values of *top*, *right*, *bottom*, and *left*. The oddset does not affect the position of any other elements.
  - This value always creates a new **stacking context**. 

# Transitions

Transition: 
Property name | Duration | Timing Function | Delay

# The Power of CSS Transform

```CSS
transform: rotate(45deg);
transform-origin: top left;

transform: scale(0.5);
transform: translateX(200px);
transform: translate(50px, 50px);
transform: skew(30deg);
transform: skew(5deg, 5deg);

transform: rotate(-20deg) scale(2);
```

We can change the orgin of the transformation of elements

# The Truth About Background

```css
background-image: ;
background-size: ;
background-repeat: ;
background-position: ;
```

background-size:
- contain
- cover
- etc

background-repeat:
- repeat-x
- repeat
- no-repeat
- space
- round
- space repeat

background-position:
- top
- left
- center
- 25% 75%
- bottom 50px right 100px
- right 35% bottom 45%

background
- the order doesnt matter, except one case where we are required to use /

- we can have multiple backgrounds

# Google Fonts are amazing

