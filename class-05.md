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
                  <img src="childfolder/imagefile.jpg" alt="This is an example description" title="This is an example title" width="300" height="300" />
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
            
        
          
