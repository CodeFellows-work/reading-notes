# HTML Links, JS Functions, and Intro to CSS Layout # 
## Links ## 
There are several ways to use links within HTML. There is a method to link to another website, a method to link to another page that is part of the same website, a method to link to a part on the same page, a method to open up a new browser, and a method to start up your email program and send an email to someone. 

### Linking To other Websites ### 
What you must first understand is the beginning part of a link. The beginning part of a link will use the `<a>` element followed by an `href` to make the link. Here is an example: 

      <a href=""... 
   
As mentioned in previous notes, the <a> element or tag is called the anchor tag. So to link to another website you will need the full address of the website you want to link to. This is called an **absolute URL**. This is an example: 
  
       <a href="githiub.com"> Text you want to make a link </a> 

### Linking To Another Page On The Same Website ### 
To link to another page on the same website - and an example for this can be like a contact page, or an about us page, you you can use what is called a **relative URL**. Makes sense because the main page is like a parent page, and the other webpages you want to link to which are on your same website can be like child pages. An example for this link can be simply your webpage address that you created. 

      <a href="myexamplewebsite.html"> Text you want </a> 
   
### Directory Structure ### 
Within a larger website it is a good idea to organize your files. Maybe creating files and putting each webpage into another file that will branch from your main webpage. For instance: 
                  
              ( This is a parent )
      Main Web Page----->     |----------------------->  sub page folder  ( This is a child )
         folder               |----> image folder         |
            |                 |                           |
         index.html         images                  another folder within sub page   <----|
                                                          |                               |
                                               content for sub page.html             ( This is a grandchild )
                                               more content.html                          
   
So all of these files can be linked to within your main web page or the parent as seen in the example, and you do not require the full link to link them into your main web page. You can use what is called **relative URLS** 

Relative link Type | Example 
-------------------|---------
Same folder | just use the file name 
child folder | name of the folder with a foward slash 
grandchild folder | child folder followed by a foward slash then the grandchild folder name followed by another foward slash
parent folder | use ../ to indicate the folder above that one and then that is the name
grandparent folder | just like the parent folder use the ../ but twice and then you will see the name 
                   
### Email Links ### 
To use an email link you can just use the anchor tag with href to `mailto:` followed by the email address. 
      
      <a href="mailto:exampleemail@example.com"> Email Me </a> 
### New Window ### 
If you want to make a link open on a new window just follow your anchor tag and href link with a `target="_blank"`. This is how that would look like: 
            
         <a href="github.com" target="_blank"> This is a link to GitHub that will open in a new window </a> 
### Linking to parts of a page on the same page ### 
To link to something that will direct the user to another part of the webpage within the same webpage, you simply create an id to the element you want to link and then mention the id in the <a> tag. For instance 
      
      <h1 id="ThisIsWhereTheLinkWillTakeMe"> This is the part you will see when you click the link </h1> 
      . 
      .
      .
      .
      <a href="#ThisIsWhereTheLinkWillTakeMe"> go to header 1 link </a> 
      
## Layout ## 
Here we will check out different ways to create good looking layouts for your webpage. There are multiple methods to position your elements make them look good on your webpage. 

### Positioning ## 
first let's tkae a look at positioning. 
 * Normal Flow 
      * `position:static` 
      * In normal flow positioning, all the text will just sit right on top of each other and is the default look.  
      * syntax not needed as this is the default. 
 * Relative Positioning
      * `position:relative`
      * Relative positioning essentially keeps the style of the normal flow positioning, but you are able the block around. 
 * Absolute Positioning
      * `position:absolute` 
      * When you use absolute positioning, it does not affect other elements on the page. The other elements act like this chunk is not there. 
 * Fixed Positioning 
      * `position:fixed` 
      * This positioning is like the absolute positioning but it is affected by the browser window. If you use this positioning the element will stay put even if a user scrolls up or down. 

An element worth noting, for the sake of layouts is the **floating element** or `float`. With this element you can take normal flow element and place as far to the left or right as possible while still keeping the content. 

## Functions ## 
A better way to organize your JavaScript is through the use of functions & methods, objects, and built-int objects. But our main quest for these notes are functions. 

So what are functions? Functions are essentially a way to group your statements and put it into one method. This way you can potentially eliminate writing thousands of lines of code. Just like how we store values in variables, functions are like storing statements. 

So when you want to use this function later in your code, you must ensure to call it. To do this you create a name for your function so that you can **call** it later. To go through the motions and relay the gist of the creation of a function you must start off by declaring the function and giving it a name. Then you enter the block of code you want it to run (when information is passed through this block of code it is known as **paremeters**). When your function gives you back the information that you needed, it **returned** a value. This is how the code can look: 

            
            function exampleFunction('parameters go in here') {
            ^-----^  ˆ---------------ˆ
               |              |
    this is function keyword  |
                              This is the declared name of the function
                  console.log('hello this is an example');
                  ^--------------------------------------^
                                                |
                                                ------------- This is the code inside the brackets that will execute when called
                  }
                  
                  function(); 
                  ^--------^
                        | 
                        Calling the function to run 
                        
Note that the block of code will not run until the function has been called. So let's say that I declared a width with a value and a height with a value and want to know the area of a square. This might be how it will look like: 
            
            let width = 2;  // set the variable width to 2
            let height = 3; // set the variable height to 3 
            
          function area(){ //made my function 
           area =  width * height;  // entered what the function will do 
           return area; // made the function return the value 
           } 
           
        function(width,height); // none of the code will work until I call the function 
        
I can also create functions in a variety of different ways: 
            
            function example() { // Function declaration 
            }
            
            let example = function(){ // Function Expression 
            } 
            
            let example = ((function() { // Immediately Invoked Function Expression (IIFE) 
            }
            ()) 
 
## Pair Programming ## 
As you may have heard, multiple minds make greater achievements (or something along those lines). If it did not work, you probably would not hear about it. 
So what if we had multiple people, working on code? I can understand if there is conflict, but overall I think it can be very efficient. 

"Research indicates that pair programing takes slightly longer, but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging (let alone exposing users to a broken product). So, in the long-run, it’s often actually more efficient than two people working on separate features." source: https://www.codefellows.org/blog/6-reasons-for-pair-programming/ 

Not only will your code become more "higher-quality" but it gives you a chance to make collaberative ideas. There has to be a time where you and some of your buddies got together and genuinly though up of a good idea... Maybe not when your drinking. 

You also will be able to learn from each other. Unlike in a classroom environment where you could be dozing off, working with a buddy and engaging each other can result in picking up a few things from each other. Not only can you learn but you also have a chance at socializing and you know what that means... it's very possible to network this way. 
You never know where the person you are collaberating with will be in the near future. Maybe this person can give you an opportunity that you have always dreamed of. 
Working with someone can also help your job interviewing skills, because you are almost forced to think on the spot and your partner(s) might push you to do this. I think at least this is a good environment to grow intellectually. Lasty, don't forget, when you find your next job as a software developer - your not going to be programming alone. So it is a good idea to get used to the motions of working with people when coding. 
