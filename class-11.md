# Audio, Video, Images # 
As mentioned in previous notes, images can make your web page pop and attract the attention that it deserves. We can can now control image positions with CSS, and keep it out of the HTML portion. 

## Sizing Your Image ## 
To start off, within CSS, you can control the sizing of an image using the width and height properties. This is a practice or habit to form when controlling images on CSS because, using this can actually make your web page load faster. This is because when the browser loads, the HTML and CSS load first and dictating how big the width and height will tell your browser how much space to reserve before your images load. 

## Aligning Your Image ## 
An increasingly popular method with developers is to use the float property to align your images within the web page, instead of using the images or <img> align property. 

## Center Your Image ## 
Remember that image elements are inline elements, meaning the images will flow within the surrounding text. Therefore, before you want to center an image you should consider changing your image element into a block element, using the property **display** and adding the calue **block**. Furthermore, there are multiple ways you can center your image. One way is to center the image on the element itself, using the left and right margin properties and setting both of them to auto. Another method is to set the containing element of the image using the **text-align** property. 

## Make Your Image into a Background ## 
If you want a particular section, or maybe even the whole page to have a specified background image you had in mind - you can always use the **background-image** property on any element.

## Repeat Your Images on the Page ## 
To enable your background image to fill out a giant space (let's say), or you simply just want your image to repeat and fill the entire space. You can do that by using the **background-repeat** property. This works well with designs that you may want to show conitnuously throughout your web page. The background-repeat property also has 4 values that it can take. They are:
  
  1. repeat /* background image will repeat both horizontally and vertically, throughout your web page. */
  2. repeat-x /* background image will repeat horizontally */ 
  3. repeat-y /* background image will repeat vertically */ 
  4. no-repeat ?* background image will only be shown once */

There is also the **background-attachement** property you can use to dictate whether you want your image to remain where it is, or scrolls when the user scrolls. This property is pretty neat. So along with background-attachments property, the values that it will take in include: 
  1. fixed /* will remain in the same position on the page. */ 
  2. scroll /* will scroll along with the user *./ 

## Position Your Background Image ## 
So, how about poisitioning your background image. We already wen over how to position your images, but not background images. So to fdo this, we can use the property **background-position**. This property will position your background image to the values you set it. This includes: 
  1. left top 
  2. left center
  3. left bottom
  4. center top 
  5. center center 
  6. center bnottom
  7. right top 
  8. right center 
  9. right bottom 

If that is too long for you to remember, you can always use the shorthand version which will just use the property **background**.

## Image Rollover and Sprites ## 
Another interesting design you can incorporate into your web page is styling the buttons on your page with different images. Just as how you can change the colors of your links whenever they are not clicked, clicked, or active - you can achieve the same but with images. When using one image such as a logo - which is used over and over again on your web page, this is called a sprite. 
Sprites are a good thing to use because this will actually speed up the browser loading speed - because the browser will only look for one image. 

## CSS Gradient ## 
What about those cool images that fade into another color? CSS can do that too. This is called a CSS gradient. You set the gradient by using the property **background-image** and then set the value to some kind of gradient. This is a relatively newer style so older browsers may not be able to do this. 

# Practical Information # 
When thinking about your web pages success you may want to further your knowledge on **SEO** or **Search Engine Optimization**. This term generally means to make your web page near the top of a search result in order for your web page to attract more attention, or ultimately to be found. To improve your chances of this, you need to consider the 7 different things that can better your chances of search results. The browser will look at the 
  1. Page Title 
  2. URL/ web address 
  3. Headings
  4. Text 
  5. Link Text
  6. Image Alt text 
  7. and Page Descriptions 

I would say to do some research about key words and use those keywords, and try to incorporate them into your web page so that you can expect more customers on your page. 

Also, get to know and understand your visitors. For instance, try to understand their thought process and their process in general in terms of how they reached your sight to begin with. You can use this knowledge to your advantage to make adjustments to your web page so it becomes more easily discovered. You can sign up for analytics on google.com/analytics to put tracking code into your web page. This will give you information such as: 
  1. Visits 
  2. Unique visits 
  3. page views 
  4. pages per visit 
  5. average time on your sites 
  6. data selectors 
  7. export the stats 

Furthermore, you will need a domain name and hosting service to hold your web page. 
