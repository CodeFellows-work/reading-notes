# <ins>HTML Text, CSS Intro, Basic JavaScript</ins> # 
## HTML Text ## 
These notes will expand more on the elements used for HTML or the **markup** text that is used within HTML. To get started, there are two types of markup styles. 
* Structural Markup 
  Structural Markup is used to specify headings and paragraphs. These elements look like this `<h1> This is a heading </h1>` 
`<p> This is a paragraph </p>`
* Semantic Markup 
Semantic markup can be seen as something that is used in between those elements to give more detail or to emphasize something that might be within the content you are providing. We will go over the markup for that shortly. 

### Headings ### 
HTML uses a set of 6 headings with all different sizes `<h1>`being the largest and `<h6>`being the smallest. 
![Heading sizes](https://www.tutorialrepublic.com/lib/images/html/html-headings.png)

Source: 
HTML headings. (n.d.). Retrieved April 05, 2021, from https://www.tutorialrepublic.com/html-tutorial/html-headings.php

`<h1>` mainly used for the main headings while the rest of the headings are more for subheadings. A paragraph element will contain one or more sentences, and a start of a pragraph will always start on a new line. This is a paragraph tag: `<p> </p>`. 
What we covered so far are some structural markups. The headers and the subheaders, as well as the paragraphs which form sentences on new line (everytime a pragraph tag is used). 

### Bold and Italic ### 
To make words appear in **bold** lettering, in HTML you use the `<b>` element to wrap around the word that you want to make bold. This is an example of a *semantic* markup. 
To make words appear *italicized*, in HTML you use the `<i>` element to wrap around the word that you want to make italic. This is another example of a *semantic* markup. 

### Superscript and Subscript ### 
Let's say you want to include a math equation and it includes an exponent. The **superscript** or the `<sup>` element is the go to. For instance if you wanted an output for "x squared" your code will look like 
 
      <p> The formula includes x<sup>2</sup></p> 
This can also work for dates. 

Let's say you wanted to use CO2 for a chemestry assignment. This would call for a **Subscript** or `<sub>`. The code for the proper way to write CO2 would look like this: 

      <p> There is too much CO<sub>2</sub></p>
      
### White Space ### 
When there are mutliple spaces next to each other in between words, this is known as **white space collapsing**. Sometimes developers will do this so that a piece of code is easier to read. The example that will be shown will have code with white spaces, however the output of the code will remain the same as if the spaces were not there in the first place. 

        <p>This is a sentence</p> 
        <p>This    is a sentence</p> 
        <p>This       is a    sentence</p> 
        
### Line Breaks aand Horizontal Rules ###
How about using the same paragraph but starting some words on a different line? That is what the `<br>` tag or **break** tag can be used for. This is an example: 
         
         <p>This is all <br />going to be within the same <br />paragraph element but some <br />words will be on different lines</p>
         
The example above will have the the paragraph ouputted like so: 

          This is all 
          going to be within the same 
          paragraph element but some 
          words will be on different lines 
          
How about if we wanted to input a horizontal line in between two paragraphs? The <hr /> tag or **horizontal rule** tag will be used for this. This is an example: 

          <p>This will be a sentence above the horizontal line</p>
          <hr /> 
          <p>This will be a sentence below the horizontal line</p> 
          
The output would look like this: 

          This will be a sentence above the horizontal line
          _________________________________________________
          This will be a sentence below the horizontal line

### Strong and Emphasis ###
The `<strong>` tag or element is used to emphasze whatever is wrapped in between this element to show that it has a strong presence. Therefore, when using this tag, the word that is wrapped in between will output in bold lettering. 

The `<em>` or **emphasis** tag has the ability to change the meaning of a sentence. Wrapping the `<em>` tag around a word will output the word as *italicized*.

### Quotations ### 
To markup quotations you can use two elements. One of the elements used is called `<blockquote>`. This element is generally used for longer quotes that could even take up a whole paragrpah. If a block quote is used, it proabably also will be indented (though it should be noted that you should not use the blockquote just for indentations. CSS should be used for regular indents). This is how you can use a `<blockquote>`: 

            <blockquote cite="https://www.example.com"> 
              <p>whatever is being quoted</p> 
             </blockquote> 
             
 Another method to quote things, is for a smaller quote. You use the `<q>` element to quote smaller quotes. For instance, 
              
              <p>This will be a sentence before the quote. <q> This is the quote </q></p>
              
 ### Abbreviations and Acronyms ### 
 If your webapge is going to use a lot of acronyms or abbreviations and you dont want to utilize your paragraph to constantly cover what those acronyms or abbreviations stand for, you can simply just use the `<abbr>` or the `<acronym>` element. This will show the definition or the full text on mouse hover. This is how you can use it: 
 
        <p>I work for the <acronym title = "Centeral Intelligence Association"> CIA </acronym> </p> 
     
 Now when hovering over "CIA" the description or what was written in between `<abbr>` will show. `<abbr title="..."> </abbr>` is HTML5 form and `<acronym title ="..."> <acronym>` is HTML4.  
 
### Citations and Definitions ### 
The `<cite>` element is used to depict where something is from. For instance, 

          <p><cite>To Kill a Mockingbird</cite> by Harper Lee</p> 
          
 Whatever is in between the `<cite>` element will show italicized. 
 
The `<dfn>` element is used to indicate a meaning for a new term. Browsers will show whatever is wrapped in between `<dfn>` as italicized, but Safari and Google Chrome will remain as is. 



