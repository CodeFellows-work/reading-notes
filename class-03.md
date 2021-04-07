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

### Width ### 

