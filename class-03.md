# <ins>HTML Lists</ins> # 
In HTML there are a couple of ways to create lists. There is a way to make a list that is numbered in numerical order, there is another way to make a list that will show as bullet points, and finally there is a way to make a definition list. 

      <ol> <!-- This element is used to create something called an "ordered list". Hence the element uses the letters "o" and "l". 
        <li> Text in here will be leading after a "1."  </li> <!-- the <li> element means list and will be nested in either a ordered list or an unordered list. --> 
        <li> Test in here will be leading after a "2." </li> 
      </ol> 
      
      <ul> <!-- This element is used to create something called an "unordered list". Hence the element uses the letters "u" and "l" --> 
        <li> Text will be leading after a bullet point </li>  <!-- notice that the <li> element is used again --> 
        <li> Text will be leading after a bullet point </li> 
      </ul> 
      
      <dl> <!-- notice that this list is a lot different than the other types of list. This uses the letters "d" and "l" as in definition list--> 
        <dt>This will be the term you are defining</dt> <!-- this uses the letters "d" and "t" as in definition term --> 
          <dd>This is where the definition will exist</dd>  <!-- this uses the letters "d" and "d" as in definition defined --> <!-- the <dt> and the <dl> elements will be                                                                                   nested in between the <dl> element --> 
       </dl> 
       
Other things you should note is that you can nest another list inside of another list. **This is called nested lists**. For example: 

        <ul> 
          <li> item 1 </li> 
            <ol>
              <li> trait for item 1 </li> 
            </ol> 
        </ul> 

# <ins>Boxes</ins> # 
As you may know by now how CSS treats all HTML elements as if they are in their own box - now we will take a look at how we can style these boxes. 

## Box Dimensions ## 

### Height and Width ### 
To change the sizing of a box, you can change it by using the width and height properties. Using these properties you change the values of those properties by using a number folllowed by either using **px**, a **percentage**, or **em**. Most developers will opt to use the px because you can accurately define the size using it. When using percentages note that it is the **percentage** or size relative to the size of the browser window, and if the box is within another box it is the size relative to the containing box. 
When using **ems**, note that the box size is relative to the text size within it. Here is an example of how they are used: 

             div {                        <!-- element <div> uses the px to size its surrounding box --> 
                  height: 30px;
                  width: 30px; 
                 } 
                 
            div {                         <!-- element <div> uses the percentage to size its surrounding box --> 
                  height: 30%;
                  width: 30%;
                  }
                  
            div {                         <!-- element <div> uses the ems to size its surrounding box --> 
                  height: 30ems;
                  width: 30ems; 
                  } 
                  
You can also limit the size of the surrounding box by attaching the "min" or "max" before width or height. Like this: 

                        div {
                        min-height: 30px; 
                        max-width: 30px; 
                        }
                
### Overflow Content ### 
When the content that is in your box comes out to be larger than the box itself, there is a solution for that. You can use the hidden property which will hide any content that does not fit in the box, or you can you uise the scroll property so that users can scroll through the box to see the rest of the content. Here is how that is written in code: 

               div {
                  overflow: hidden;
                  }
                  
              div {
                  overflow: scroll;
                  }
### Border, Margin, and Padding ### 
Every box has a border whether you see it or not and will seperate the edges of a box with another. A margin is the space just outside of the border and can seperate the set box from another box. Padding is the space that is in between the text and the border. Just as how you set the width and height, you can set these in the same way. "margin", "border", "padding". 

### Border Width, Size, Color ### 
The **border-width** property can be used to set the width of a border. To set the value of the width you can use a number followed by the **px** or pixels or you can use the following values:
* thin
* medium
* thick 


In addition to setting the values, you are also able to specify where you want to set the width using: 
* border-top-width 
* border-bottom-width
* border-left-width
* border-right-width


Now that you can change the width of the border, how about the styling of the border. With the **border-style** property you can make your border look more catchy using the following properties: 
* solid - this will result in a solid lined border
* dotted - this will result in a dotted line border
* dashed - this will result in a dashed line border
* double - this will result in a solid double lined border
* groove - this will result in a border that looks like it is carved into the page
* ridge - this will result in a border that looks like it sticks out from the page 
* inset - this will result in a border that looks like it is sinked into the page
* outset - this will result in a border that looks like it pops out from the page
* hidden / none - this will result in a border that you can not see


And you can change the style of the border individually as well just like the width using: 
* border-top-style 
* border-bottom-style
* border-left-style
* border-right-style

Another property you might want to add to the border is color. **border-color** is used to change the color of the border. Again, you can individually assign colors to each border line. 
* border-top-color
* border-bottom-color
* border-left-color
* border-right-color 

Let's say you don't want to write all the properties on a new line. There is also a solution for that! Short hand border properties allow you to set the width, style, and color, using only one property. Here's an example: 

      div {
      border: 3px dotted black; <!-- 3px is the width, dotted is the style, and black is the color of the border --> 
      }
      
As mentioned before, padding is the space that is controlled from the text inside the box to the border. You can set these indivually as well using: 
* padding-top 
* padding-bottom 
* padding-left
* padding-right 

The same concept applies to margin: 
* margin-top 
* margin-bottom
* margin-left
* margin-right 

### Centering Content ### 
Now let's say you don't like the look of your box on the left or you simply need to move the box to the center. To do this you must set the width of the box because if not the box width will just take up the entire page. So once you set the width of the box, you can use **left-margin** and **right-margin** and set them both to auto. 
To make this work on older browsers you may need to include the **text-align** and set its value to auto as well. *The tex-align property is inherited by child elements* 

### Change Inline/block ### 

Using the **display** property you can turn an inline element into a block element or vice versa. You can also use the **display** property to hide elements within a page. This is how you can use the **display** property: 
            
          li {
           display: inline; <!-- makes a block element act inline --> 
          } 
          
          li { 
          display: block; <!-- makes an inline element act like a block --> 
          } 
          
          li {
          display: inline-block;    <!-- makes a block element act like inline while maintaining the properties of a block --> 
          }
          
          li{
          display: none;      <!-- hides an element from the page --> 
          } 
      
### Hiding Boxes ### 
You can utilize the **visibility** property to either hide or show the element. Note that when hiding the element the element will still be there but nothing will appear resulting in a gap or blank space. Example text:
      
            li {
            visibility: hidden; <!-- hides the element --> 
            }
            
            li {
            visibility: visible; <!-- shows the element --> 
            } 

## CSS3 ## 
### CSS3 Border Images ###

CSS3 introduces (in my opinon) cooler ways to style the border of a box. Using the **border-image** you can use images to be a border of any box. To use the **border-image** property three things must exist however. **border-image** will require 
1. the img URL
1. where to slice the img
1. and what to do with the straight edges
      * stretch - which stretches the img
      * repeat - which repeats the img
      * round - acts like repeat but scales the tile img if it does not fit 

The box width must be assigned or else the border image will not show. 

### CSS3 Box Shadows ### 
The **box-shadow** property works just like the **text-shadow** property but it is for boxes - it will add a drop shadow to your box. The **box-shadow** property must use atleast the first two of the values presented as well as a color for it to work. 
* horizontal offset - negative values position the shadow to the left of the box
* vertical offset - negative values position the shadow to the top of the box 
* blur distance - shadow is like a solid line like a border if omitted 
* spread of shadow - a positive value will spread the shadow 

## Rounded Corners On Boxes ### 
Using the **border-radius** property, you can round the corner edges on any box. Note that this will not work with older browser as they do not support this property. If this property is not supported the boxes will just end up being right angles. You can also specify which corner to round like this: 
* border-top-right-radius
* border-bottom-right-radius
* border-top-left-radius
* border-bottom-left radius

The cool thing about the **border-radius** property is that you can also make shapes using this property. By changing the values around for each edge you can create evena  circle! 



