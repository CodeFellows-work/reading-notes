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

### Author Details ### 
The `<address>` element can be used to store your contact information. IT can have a physical address, a link to your email, or contain your phone number. It is like the business cards of HTML. 

        <address> 
          <p><a href="mail to: example@example.com"> 
          example@example.com</a></p> 
          <p>1111 example address</p> 
        </address> 

### Changes to Content ### 
A `<del>` element will show a word that is wrapped in it with a strike-through to show that the word has been deleted from the content. 
A `<ins>` element will show a word that is underlined to show that the word has been newly inserted in the content. 
Similarly, the `<s>` element will show a word that has a strike-through to show that the word is no longer relevant (could be used for an ad). 

## CSS Introduction ## 
CSS will allow you to change how words and backgrounds of your content, will look like. For instance, you can align your text in a specific way, change the color for each header, or paragraph, change the fonts, sizes of fonts, font color, etc. CSS will be used extensively when making your website look pretty. 

When using CSS it is best to imaging that within every element there is an invisible box, and within that box you have the power to change the way that element will look. 

### Selector and Declaration ### 
Within CSS there are two parts. The **selector** (which will select which element you want to style) and the **declaration** (which will let you choose the style for the element. For instance,
  
          p {     <!-- curly brackets will be used when using the selector and declaration inside of the curly brackets --> 
            font-family: sans-serif;     <!-- font-family is used to determine the font you are going to use, sans-serif is the font used in this example --> 
            }                            <!-- in CSS after the declaration, a semi colon will be used to specify that it is the end of your code --> 
        
Within the declaration there are two more parts. The **property** and the **value**. In the example shown above **font-family** is the property and **sans-serif** is the value. 

### Using External Links for CSS ### 

A `<link>` element followed by three attributes will be used within the `<head>` element if you want to specify a style that is found externally. The element is empty just meaning that there is no closing tag for this element when used. The attributes `href`, `type`, and `rel` are used along with the `<link>` element. For instance: 

        <head> 
          <title> Example external link </title> 
            <link href="css/styles.css" type="text/css rel="stylesheet" /> 
        </head> 
        
 `href` specifies the link, `type` specifies what the document that is being linked to and `ref` specifies the relationship between HTML and the file that it is linked to. 
 
### Using Internal Links for CSS ### 

You also have the options to set rules for an HTML page with CSS internally by using the `<style>` element which will usually sit in the `<head>` element. When using this method ensure that the attribute `type` is used which equals to `"text/css"`. This indicates that the style is specified in CSS. 

      <head> 
        <style type="text/css"> 
          body {
            font-family: sans-serif; 
            } 
          </style> 
       </head> 
     
 ### CSS selectors ### 
 Selectors will let you choose where to style. 
 
 Selctor   |   Example 
 ----------|----------
 Universal | `* {} ` selects all elements on the page
 Type Selector | `h1, h2, h3 {} ` Targets `<h1>` `<h2>` `<h3>` 
 Class Selector | `.example {}` Targets whatever element that uses the `.example` class 
 Id Selector | `# example {}` Targets id's with the id of `# example` 
Child Selector | `li>a {}` Targets any `<a>` element within the `<li>` element and only within the `<li>` element 
Descendant Selector | `p a {}` Targets the `<a>` element that is nested in the `<p>` element along with anything else inside the `<a>` element 
Adjacent Sibling Selector | `h1+p {}` Targets the first `<p>` element nested in the `<h1>` element and nothing else
General Sibling Selector | `h1~p {}` Targets more than one `<p>` element nested in the `<h1>` element 

### CSS Rules Cascade ### 

So CSS has a set of rules meaning CSS has an order of precedence. If you have to of the same selectors, CSS will choose the latter of the two - meaning the second rule will be chosen over the first one. A better way of understanding is - the most recent rule you have incorperated will take precedence. This is called the **Last Rule**. 

Another rule CSS abides by is with **specificity**. Meaning CSS will take the rule that is more specific over the one that is less specific. 

A way to make sure that CSS will override this rule is by using the `!important` after the property value to ensure that this rule will take all precedence. 

### Inheritance ### 

If you specify a `font-family` or `color` properties they will apply to most of the child elements, and that is because these properties are inherited. This makes for a simpler way of styling your sheets. On the other hand `background-color` or any border properties will not be inherited, and if they were your style sheets can look very messy. You also have the option to force inheritance to a property by adding `inherit` so that the properties can inherit the values of its parent element. 

## Basic JavaScript ## 
Within these set of notes, we will discuss how to read JavaScript, as well as how to give your webpage a set of instructions to follow to make it more interactive with its users. 

### Statements ### 
Something to note before we continue is that JavaScript is case sensitive. `exampleJava` is completely different than `ExampleJava`. 

Each statement always starts on a new line and will end with a semicolon. Either way this makes JavaScript easier to read so it is a good rule. The semi colon basically tells the JavaScript editor or interpreter that the statement is complete. Here is an example: 

          console.log("Hello Code Fellows!");  

Some statements will include code blocks which is basically code that is surrounded by curly brackets. Semi colons are not used after these curly brackets. Here is an example: 

          if(var i = 0; i < 3; i++) {
            console.log(i); 
           }
 
 Code blocks is a good way to organize or group together many statements. This also helps the code to be more readable. 
 
 ### Comments ### 
Remember in HTML to comment you use `<!-- this is the commment -->`. However in JavaScript to comment you simply need to do `//`. Again comments are a good way to help someone that is reading your code understand your code, as well as keep yourself organized so that you can go back to what you have written and understand what the code will do without trying to figure it out all the time manually. 

### Variables ### 
**Variables** are what you use to store information. This is very useful because with the stored data you can add more information and use those variables to keep storing data without having to manually write code for every bit of information you need. Let's use the example code above. The variable "i" has the value of 0 stored. Everytime  the if statement runs (as long as "i" is less than 3), the variable "i" will add 1, and also log to the console. This is a better and more efficient method than to `console.log` everytime manually until "i" is greater or equal to 3.

So how do we use variables? First use var in front of the variable name you want to use to define a variable. 

        var example;
    
As you can see, we have made "example" a variable. Now we have to assign a value to this variable. 

        example = 0; 
        
Notice that I did not include `var` when assigning the value to the variable. This is because the code snippet above this example already declared this variable as "example". Of course you can also make this one line making it: 

        var example = 0; // this is called a shorthand method 
        
 ### Data Types ### 
 In terms of JavaScript and other high-leveled programming languages, there are different data types. In JavaScript there is **Numerical** data types which include positive integers, negative integers, as well as decimal integers. There is also the **String** Data type which consists of any letter or character as long as they are wrapped in quotes. Lastly there is **Boolean** data types. This data type is simply going to be a true or false. 
 
 ### Combine ### 
 
Now lets store each of the data types covered into a variable. 

        var number; //storing a number value in a variable 
        number = 12; 
      
        var word; //storing a string value in variable 
        word = "hello"; 
        
        var fast; //storing a boolean value in a variable 
        fast = false; 
        
As seen in the code snippet under the "statements" subheading, you will notice that a variable can change with code written later. A variable does not have a fixed value and can change. 
 
### Rules For Naming Variables ### 
1. The name must begin with a letter and not a character or a number.
1. The name can include numbers, letters, a dollar sign, or an underscore, but no dash or period.
1. The name cannot be a keyword or a reserved word which is part of the language of JavaScript. For instance, your variable cannot be named var. 
1. Remember that all variables are case sensitive.
1. Use a name that resembles the values that will be stored in the variable, for instance "firstName" for a persons first name. This keeps everything organized. 
1. Remember to use camel case lettering. So if the varible is more than one word use a smaller case to start and a captolized letter for the second word. ex. "firstName"

### Arrays ### 
If you have multiple values you wish to store in one variable, then an **array** is a perfect solution. Arrays can store multiple values in one variable. This is how multiple values can be stored in a single variable: 

        var numbers; 
        numbers = [1,2,3,4,5]; 
        
This method of creating an array is called an **array literal**. Another method or technique you can use to create an array is called a **array constructor** which uses the `new` keyword followed by `Array();` with the values stored in between the parenthesis. This is how it looks: 

        var numbers = new Array(1,2,3,4,5); 
        
 You can also write the values on a new line for every value just so long as it is within the parenthese or brackets. 
 
When defining a value in an array, each value is stored within a number plane starting with "0". For instance the code snippet above in the array "numbers" the first value of the array is assigned in the "0" spot, and then the next value in the "1" spot and so on. So to call a specific value within the array you can use the variable name and the spot that the value is in surrounded by square brackets. For instance: 

        numbers[3]; // This will call the 3rd place within the array which is the value "4" 
        
This is how computers start counting. What else can you do with arrays? You can change their values by using the method that was just shown to call a specific array. For instance let's say I wanted to replace the 2nd value with a different value. 

        var numbers = [1,2,3,4,5]; 
        
        //update the array
        numbers[2] = 10; 
        
By doing this I just made the value "3" into "10". 

### Expressions ###


      
    
