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
* solid 
* dotted 
* dashed
* double
* groove
* ridge
* inset 
* outset
* hidden / none 


And you can change the style of the border individually as well just like the width using: 
* border-top-style 
* border-bottom-style
* border-left-style
* border-right-style

                  
