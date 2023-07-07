### CSS Selectors  
| Selector | Example | Description |   
| ------- | -------| ---------|  
| #id | #firstname | selects all element with id="firstname" |  
| .class | .intro | selects all element with class="intro" |  
| element.class | p.intro | selects ```p``` elements with class="intro" |  
| * | * | select all element |  
| element | p | select all ```p``` element |  
| element, element,... | p, div | select all ```p``` and ```div``` element |  

### How to add CSS  
- External CSS : ```<link rel="stylesheet" href="mystyle.css">```  
- Internal CSS : ```<style> all css style here</style>```  
- Inline CSS : ```<element style="desired style" > content </element>```  

### Cascading Order  
- Inline style (inside an HTML element)
- External and internal style sheets (in the head section)
- Browser default

### CSS Comments  
```/*comment here*/```  

### CSS Colors  
```
h1{
    background-color: lightblue; /*background color*/
    color: red; /*text color*/
    border: green; /*border color*/
}
```  
Color adding format:
```
    rgb(255, 99, 71),
    #ff6347,
    hsl(9, 100%, 64%),
    rgba(255, 99, 71, 0.5),
    hsla(9, 100%, 64%, 0.5)
```  
Color picker : https://www.w3schools.com/colors/colors_picker.asp  

### CSS Backgrounds  

- background-color: value;
- opacity: value; [value from 0.0 to 1.0]
- background-image: url(link_here);
- background-repeat: repeat-x; [or repeat-y or no-repeat]
- background-attachment: scroll/fixed/local/inherit/initial/revert/revert-layer/unset;
- background-position: value;
- background (shorthand property)

For example :  
```
    body{
        background-color: green;
        opacity: 0.3;
        background-image: url(paper.gif);
        background-repeat: repeat-y;
        background-attachment: fixed;
        background-position: right top;
    } 
    
    For shortand : 
    body{
        background: green url(paper.gif) repeat-y fixed right top;
    }
```  

### CSS Borders

- border-style: ``value``; [dotted/dashed/solid/double/groove/ridge/inset/outset/none/hidden]
- border-width: [``value``] or [``value`` ``value``] or [``value`` ``value`` ``value`` ``value``]
- border-color: [``value``] or [``value`` ``value``] or [``value`` ``value`` ``value`` ``value``]
- border-top-style: dotted;
- border-right-style: solid;
- border-bottom-style: dotted;
- border-left-style: solid;
- border-radius: value;
For example : 
```
    h1{
        border-style: dashed;
        border-width: 5px;
        //border-width: 5px 6px;
        border-radius: 2px;
    }
```  

### CSS Margins  

- margin-top
- margin-right
- margin-bottom
- margin-left
<!-- All the margin properties can have the following values:

auto - the browser calculates the margin
length - specifies a margin in px, pt, cm, etc.
% - specifies a margin in % of the width of the containing element
inherit - specifies that the margin should be inherited from the parent element -->

```
    selector{
        margin: value;(all sides)
    }
    selector{
        margin: value(top) value(right) value(bottom) value(left);
    }
    selector{
        margin: value(top) value(left-right) value(bottom);
    }
    selector{
        margin: value(top-bottom) value(left-right);
    }
    selector{
        marfin: auto;
    }

```  

### CSS Padding  
- padding-top
- padding-right
- padding-bottom
- padding-left  

```
    selector{
        padding: value;(all sides)
    }
    selector{
        padding: value(top) value(right) value(bottom) value(left);
    }
    selector{
        padding: value(top) value(left-right) value(bottom);
    }
    selector{
        padding: value(top-bottom) value(left-right);
    }
    selector{
        marfin: auto;
    }

```  

### CSS Height and Width  
- height: value;
- width: value;
- max-width: value;  

<!-- The height and width properties may have the following values:

auto - This is default. The browser calculates the height and width
length - Defines the height/width in px, cm, etc.
% - Defines the height/width in percent of the containing block
initial - Sets the height/width to its default value
inherit - The height/width will be inherited from its parent value -->  

### CSS Box Model  
![Box_Model](css_box_model.png)  

- Content - The content of the box, where text and images appear
- Padding - Clears an area around the content. The padding is transparent
- Border - A border that goes around the padding and content
- Margin - Clears an area outside the border. The margin is transparent
- The box model allows us to add a border around elements, and to define space between elements.  

### CSS Outline
![Outline](css_outline.png)  

- outline-style: ``value``; [dotted/dashed/solid/double/groove/ridge/inset/outset/none/hidden]
- outline-width: thin/medium/thick/value;
- outline-color: [``value``] 
- outline-offset: [```value```]