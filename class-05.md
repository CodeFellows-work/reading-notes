# Images, Color, Text #
## Images ## 
Images are used a lot in web pages, and why not? They help make your web page look good. We will cover how to put images in your HTML as well as which format to use for an image, making the image show at the correct size, and how to optimize your images so that browsers can load them faster. 

So to choose an image for your web page, you must ensure you ask yourself a couple questions before using a photo. Those questions are: 
 * Is the image relevant for the webpage? 
 * Does this image convey information?
 * Does this image set the right tone for your content?
 * Is this image a recognizable image? 
 * Does this image fit the style of the webpage - like color? 

Now, let's say you answered all those questons and found the right image to use for your webpage. If you are building a web page from scratch you should make a rule to yourself to create a folder just for images. This is so that you can maintain organization and easily access what you need. You also never know if your website is going to become a larger site, therefore keeping images in a folder will be very efficient and tidy. 

Alright, you got your image, and you made a file for images, now how do you add those images in HTML. To do this you use the `<img>` element or tag. Quick note, this element is an empty element meaning that it does not require a closing tag. 
After you use the `<img>` tag, you will follow it with a `src`. This essentially tells your browser where to get the image file. After the source you can add the link to the file. In most cases if your building your own webpage, this link or URL will be a relative URL such as a child folder. So far, this is how the code looks like: 

      <img src="childfolder/imagefile.jpg" 
      
After you link the image you should describe what the photo is in case the browser cannot load the image for some reason. To do this you use `alt`. I see this is as something called alternative, because it is an alternative if your image does not load. This description that you write after the `alt` will show instead of your image if your image does not load. So now, the code looks like this: 

    <img src="childfolder/imagefile.jpg" alt="This is an example description" 
    
    
Now that you have the image, the file for that image, the link for that image, put into HTML, and an alternative description for that image, you should now use a `title`. A title (with most browsers) can display your description or more information about that image on mouse hover. This is how the code looks now: 

    
    <img src="childfolder/imagefile.jpg" alt="This is an example description" title="This is an example title" />
    
## Height and Width of Images ## 
Alright, you have now included the image you wanted with the proper descriptions and titles for the images. Next is to properly size your images so that it can fit well next to the content of your webpage. Let's take a look at the `height` first. 
`height` can be added within your img element to adjust the height of your photo. We can also use CSS to change these attributes but this lesson will cover within HTML. Following the `height` you can ener a number that will represent the pixels. As a matter of fact `width` follows the same rules. By adding `height` and `width` to your `<img>` element you set the precise size for your image so that the browser knows and can render th rest of the text while leaving the perfect amount of space for which you specified in `height` and `width`. With the `height` and `width` the code will look something like this:

      <img src="childfolder/imagefile.jpg" alt="This is an example description" title="This is an example title" width="300" height="300" />
      
 As you can imagine, that image is a perfect square - and now the browser will leave just the right amount of space for this image after rendering all the text. 

### Image Placement ### 
 So where can you put these image tags? You can place image tags 
 
       * Before a paragraph <img><<p> 
       * Inside the start of a paragraph <p><img>
       * Or in the middle of a paragraph <p>......<img>

### Figure and Figcaptions ###
There are other methods to place `<img>` tags, and thhat is with using `<figure>` and then `<figcaption>` within figure. This was introduced in HTML5, and the reason was so developers can add captions to images. You can place mutliple images inside the `<figure>` as long as the `<figcaption>` element matches the caption for all of those images. The code looks something like this;

            <figure>
                  <img src="childfolder/imagefile.jpg" alt="This is an example description" title="This is an example width="300" height="300" />
                  <br /> 
                  <figcaption> caption for the example image</figcaption>
            </figure> 

### Old Code ###
Something also worth mentioning is some old code, which HTML5 does not use because CSS is taking over these methods. So in older methods you can also add the `align` attribute to move your image to the right, left, top, middle, bottom. This is not to be confused with the image itself (especially the top, middle, and bottom. What this attribute does is align the text that surrounds the image to the left, to the right, top for the first line, bottom for the line, and middle for the first line. 

## Color ## 
Without some color on your webpage, your webpage can look very dull and boring. Color is used to bring life into your webpage and set the tone for your users. 

### Foreground Color ### 
Within CSS, the `color` property is used to color the text inside an element. To set the colors however, you have some options. 

* RGB Values - RGB values will change color based on how much red, green and blue, you use within the settings. The red, green, and blue are expressed in numbers ranging from 0 to 255. So this may look like this; 
            
            h1 {
            color : rgb(100, 100, 100);
            }
         
* Hex Code - Hex code uses a hash symbol followed by a 6-digit code that will represent the color. The hex values are basically RGB but represented in a hexidecimal format. Using hex code to selct your color may look like this:

           h1 {
           color: #ffffff;
           }
        
* Color Names - Another way to change your elements colors is through names. However, the names have to be recognuzed by browsers - and are limited compared to the previous two methods. Using color names to select your color may look like this:

          h1 {
          color: blue;
          }
          
There is a good color picking tool if you go to https://colorschemedesigner.com.
          
### Background Color ### 
If you need or just want to use a background color instead of coloring your text, or maybe both - you can use the `background-color` property to set the color of the box that is surrounding your text - and this goes by element. So if I wanted to fill the background of my `<h1>` to be all blue, this is the code:

            h1 {
            background-color: blue;
            } 
            
### CSS3: Opacity ### 
In CSS3, you will begin to see properties such as `opacity`. This property enables the designer to change the element and its child elements, the opacity starting from the value of 0.0 to 1.0 or 0% to 100%. Since this is a CSS3 feature, you may not notice these changes within an older browser. You can also define the opacity using the background-color property by adding a fourth value at the end, and change the rgb properties to rgb to rgba.  The code for `opacity` might look similar to this: 

            p {
            opacity: 0.4; 
            background-color: rgba(0,0,0,0.4);
            } 
            
### CSS3 HSL, HSLA ### 
CSS3 also uses properties called `hsl` and `hsla`. These stand for hue, saturation, and light. Or hue, saturation, light, and alpha. This is another way to choose color other than RGB. Within `hsl` the hue value will be between 0 to 360 degrees, the saturation value will be expressed in a percentage, and light is also expressed in a percentage but with 0% being white, and 100% being black. 
`hsla` will add the fourth value of alpha and this is measured like opacity where the starting value is 0.0 and the last value is 1.0. This is an example of how these look ;

            h1 {
            background-color: hsl(0, 0%, 40%); 
            }
            
            h1 { 
            background-color: hsla(0, 0%, 40%, 0.4%);
            } 
            
## Text ## 
Sometimes using images, and color, are not enough to boost your confidence for a good looking webpage. How about changing the way the text looks like on your webpage. Not the color, but the styling of your text. Like different fonts, and sizes. Let's start off by changing the font of your text. 

### Font-family ### 
`font-family` is a property that will allow you to change between fonts that could be that extra push, to make your webpage look very nice. To use this property, you just need to go to the element you want to place the font change in and start by typing `font-family`. Then you can add the desired font. You can add multiple fonts seperated by commas so that if a browser does not have a font installed, it could go to the next one you specified. The code can look like this: 

            h1 {
            font-family: Georgia, Times, Serif;
            }
            
Don't think that you are only limited to the choices that your browser will give you for fonts. You can also link to fonts using the `@font-face` with a source. For instance: 

            @font-face {
            font-family: 'chunkyFiveregular';
            src: url('fonts/chunkfive.eot');
            }
            h1{
            font-family: chunkyfiveregular;
            }
            

### Font-Size ### 
If you got the font you like, you can change its size using the `font-size` property. To set the values of the font size, you can use pixels, percentages, or ems, at the end of your value. Pixels are the most precise way of sizing, percentages will go off of the default pixels that the browser uses. 
For instance, the default pixel size for a browser is 16px. if you change the percentage of a font to 75%, it would translate to 12px and 200% would translate to 32 px. ems, are dictated by the size of the text in the parent element. A good visual representation of the text sized can be seen through a word document. 8pts is like the smallest font, 72 pts is like the biggest. 

### Bold and Italic ###
just like in a word document you can bold letters to emphasize something, you can do the same in CSS. a property called **font-weight** is used to bold text. This property uses two values, one being the normal value - which will cause text to appear at a normal *weight* and then the **bold** value which will make the text bold. This is how it looks like in code:

           p {
            font-weight: bold;
            }
            
            p {
            font-weight: normal; 
            }

We also use italicized text sometimes and to do that you use the  `font-style` property. This property takes in three values which are **normal**, **italic**, and **oblique**. As you can imagine the normal value will cause the text to appear in a normal style just like it did with the `font-weight` property. The italic value causes the text to be italicezed. And the Oblique value will cause the text to appear oblique. Here it is written in code: 

            p { 
            font-style: normal;
            } 
            
            p { 
            font-style: italic;
            } 
            
            p {
            font-style: oblique;
            } 
           
### Uppercase and Lowercase ### 
Sure you can hit the caps lock key and then let yourself write your text all in uppercase... but you can do this a without having to switch your caps lock on and off. Use the `text-transform` property and then use the **uppercase** value to turn all your text into uppercase letters. Maybe you dont want to use uppercase at all even, and even if your computer auto corrected you, it would still be lowercase. 
Use the **lowercase** value to cause all of your text to view in lowercase letters. How about just the first letter? Maybe you want to to have this set automatically within an element. Use the **capitolize** value for this to occur. 

### Underline and Strike**
Let's say your designing a web page for an ad, and want to underline your selling price and strike through your old price. To do this you can use the `strike-through`property and then use the **underline** value to make the text undertlined, or you can use the **line-through** to strike through text. `text-decoration`has other values as well. 
You can use the **none** value to remove any decoration that has been set, the **overline** value to put a line at the top of text, or you can use the **blink** value to animate the text and make it flash on and off. This would be a very good property to use for ads. 

### Leading ### 
If you are familiar with a word document or even APA formatted essays, you know what double-spaced means. The vertical space that divides each line of text. You can do this on CSS by using the **line-height** property to set the verticle space in between the text - whether it is descending or closing the space, or acending meaning that there is more space.  

### Letter and Word Spcaing ### 
So we went over the vertical line space between texts or sentences, how about in-between each letter. **kerning** is the term for the space in-between each letter. You can use two properties that essentially do just that. They are `word-spacing` and `letter-spacing`. 

### Alignment ### 
Now, let's align some text. You can set the text to be all the way to the right, all the way to the left, center your text, or take up the whole width of the containing box - except the last line. To do this you can use the property `text-align` and the values **left**, **right**, **center**, and **justify** 
But now, lets say you have images stacked on top of each other and need text besides the images - it may be a situation where it looks like this: 


                        _________
                        |       |
                        | image |   'Text that needs to be next to the image'
                        |_______|
                        
                        _________
                        |       |
                        | image |   'Text that needs to be next to the image'
                        |_______|
                        
                        _________
                        |       |
                        | image |   'Text that needs to be next to the image'
                        |_______|
                        
How would you do that? You can use a property `vertical-align` to make this happen. However,  one thing to note this is more typically used with inline elements and not for block level elements. The values that are used with `vertical-align` include 
      * baseline 
      * sub 
      * super
      * top 
      * text-top
      * middle
      * bottom
      * text-bottom 

### Indenting Text ### 
Let's just say you come accross a situation where you might need to indent some text. Maybe you are quoting some text in APA format. You can use the `text-indent`property for this to occur. This property allows you to indent the first line of text to any value you choose (usually in pixels or ems). Keep in mind that this property does take in negative values, so you can push text out of the browser. 

### CSS3: Drop Shadow ### 
Because this is a CSS3 property, some old browser may not be able to view its full effects. Using a drop shadow will provide a dark version of the text behind the original text, giving it a drop shadow effect. To use this property you use `text-shadow`. This property uses four values that control where the shadow is horizontally, vertically, the blur (optional) and, finally the color. The first value indicates how far to the left or right the shadow is going to fall. The second value will indicate the distance to the top or bottom the shadow will fall,
and the third value is the blur, and the fourth value is the color of the shadow. It may look something like this on code: 

            p {
            text-shadow: 1px, 1px, 3px, #000000 
            } 
            
            
### First letter or Line ### 
If you want to only style a single line or even a single letter, you can use the `:first-letter` or `:first-line` property to do so. ONe thing to note is that this is technically not a property and its called a **pseudo-element**. This makes sense because this pseudo-element will not be in between the curly braces like properties do. Instead they will be added at the end of a selector. Like this: 

            p.example:first-letter {
                  font-family: times;
                  } 
              
            p.exampletwo:first-line { 
                  font-style: italic; 
                  } 
                  
### Styling Links ### 
If you have ever visited another web page and clicked on a link and it changed colors, that is because the `:visited` **pseudo-class** has been used. If you just seen a fancy link they used a `:link` **pseudo-class**. This is how it looks like in code: 


            a:link {
              color: examplecolor;
              text-decoration: exampledecoration; 
            a:visited {
              color: examplecolor;
            a:hover {
              color: examplecolor;
            a:active {
              color: examplecolor;
              }
As you can see these link stylers are classes and not a property. 

### Responding to Users ### 
Some more pseudo classes are used to respond to users. For instance a style that is displayed when you hover over an element, you can use the `:hover` pseudo class. Another instance can be for a style to occur if you clicked on a button, you can use the `:active` pseudo class. For any element with focus you use the `:focus` pseudo class. 

You should also note, that there is an order to using pseudo classes. The order is as follows: 
1. `:link`
1. `:visited`
1. `:hover`
1. `:focus`
1. `:active` 
