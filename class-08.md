# CSS Layout # 
## Building Blocks and Containing Them ##
To understand how the layout works with CSS you have to understnad the difference between block-level box and inline box. You should also know that CSS treats any HTML element as having boxes around them when displaying on the screen. 
* Block-Leveled Element 
    * starts on a line line ex. `<h1...h6>` `<p> <ul> <li>`  
* Inline Element 
    * continuous text, or in between surrounding text. ex. `<img> <b> 

So we have our building blocks or our lego pieces, which is the HTML elements that CSS puts a box around. Now we need to create the frame so that the elements can go into a bigger box. This is containing elements. Where block-leveled elements sit inside another block-leveled element - the outer block is the containing element. 
## Controlling the Positioning of Elements # 
There are several and different ways to begin positioning. There is: 
* Normal Flow - where all block-leved elements will appear ona new line just as the default is. 
  * `position: static`
* Relative Positioning - where this moves the element from the place where it would of been under a normal flow. Does not effect normal flow. 
  * `position: relative`
* Absolute Positioning - where this moves the element relative to the containing element. Does not effect normal flow. 
  * `position: absolute`
* Fixed Positioning - where this is another form of absoolute positioning, but the element is frozen in place and does not move when scrolling up or down. 
  * `position: fixed`
* Floating Elements - where this moves an element left or right of the containing box. 
  *  `float`

## Floats ##
To overlap onto another element you can use the property `z-index` which you can set using a number value, and the higher the number the more closer it is to the front. 

You can use float again to make multiple elements within a class to float. This can mean that all the elements or boxes would stack in the order you set it to. Make sure to use width as well. 

There is also a way to clear floats. This does not mean to wipe data, this means that the element you use the clear property with will not touch the box that is set for the clear value. 

When it comes to the parents of the floated elements - if the containing element only has floated elements, then there is a chance that some browsers will treat that has having 0 px tall. So how do you fix this issue with some browsers? You can use a couple of properties to prevent this from happening and they are the `overflow` property and the `width` property.

You can even create columns with the float. The <div> element is what creates columns, and you can call them using CSS properties to add the float property, width, and margin. 
  
## Screen Sizes ## 
When getting deeper into web developement, you should also consider the different types of devices that may access your web page. The rising advancements in technology is enableing the use of smart devices to access the internet more easily. Some screen sizes you should consider is a smart phone, a tablet, laptops, and maybe even a big monitor. 
Because of the different screen sizes and resolutions, most web developers will opt to just create a page around 960 -1000 pixels wide, because most users will be able to see the content. 
If you want to have specific options for specific types of devices, if you just want to make your webpage have a **fixed** sized web page, you can do that with **fixed width layouts**. 
This basically means that the user will not be able to change the size of the webpage even if you try to make your browser window bigger or smaller. 
**Liquid layouts** is another term that is used refarding web page screen size. This is a type of layout, unlike the fixed layout - your web page will change in size depending on the size of the browser. 

## Grids ## 
When you are designing a page, you probably already have a plan or an idea of where to place your content. You can use a layoutgrid to see how your page is lined up according to these grids. This makes for consitency and a web page that will come out to be way more asthetic than if you did not use the grid system. To place these grids on your web page you can use the **960 CSS Grid** which is a framework that comes from CSS. 
in your <head> element within your HTML, you can add a CSS grid using the link element. 
        
        <head> 
        <link rel="stylesheet" type="text/css" href="css/960_12_col.css"/>
        </head> 

Continuing on with the example of the link - as you can see we have linked a CSS style sheet into your HTML. Who says we can not add more! You can add multiple CSS style sheets you may need for different pages or even within the same page. Just use the link element to add in the link to your css stylesheet. 
