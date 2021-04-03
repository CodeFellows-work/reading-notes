# <ins>Introduction</ins> # 
---
## Accessing the Web, How it is Created, and How it Works ## 

Chances are, you have accessed the web in this day and age. Whether it is through a smart device such as a smartphone, or a tablet, or a personal computer - you have accessed the web using a **Web Browser**. 

Now there are multiple **Web Browsers** you can use to access the web. Some of them include: 

* Mozilla Firefox 
* Google Chrome
* Safari
* Opera
* Internet Explorer 

You might have a better idea if you see the logos. The following are logos of the described **Web Browsers** in order: 

![Mozilla Firefox](https://www.mozilla.org/media/protocol/img/logos/firefox/browser/logo-lg-high-res.fbc7ffbb50fd.png)
![Google Chrome](https://i.pinimg.com/originals/0a/6b/c7/0a6bc77193c559f6e6c986bbf87227c6.png)
![Safari](https://support.uakron.edu/wiki/images/d/d4/Safari-logo.png)
![Opera](https://pngimg.com/uploads/opers/opers_PNG25.png)
![Internet Explorer](http://guiadeinternet.com/files/2011/11/Internet_Explorer_9.png)

From a **Web Browser** to go to a **Web Page** you enter a web address or you can just follow a link that may be in bookmarks depending on your browser. 

### So How Does a Web Browser Access a Web Page? 

Each website or page is hosted by a server, better known as a **Web Server**. When you ask your browser to take you to a web page (such as typing or clicking on a link) your browser will send a request accross the internet to the **Web Server**. A **Web Server** is basically a computer that is specifically used to send out web pages to those that request them. 

### Screen Readers 

Another method to access the web is for people with visual impairments. Technology has now advanced far enough so that literally anyone can access it. **Screen Readers** is software that will read out the contents of a screen to a user. 

### How is it Created? 

Websites are mainly made up by `HTML` and `CSS` but can also include JavaScript. `HTML` stands for **Hyper-Text Markup Language** and `CSS` stands for **Cascading-Style Sheets**. So within the web pages that you see, your browser will be recieving the `HTML` and `CSS` from a web server and will interpret them into what you see as the web page. With a smaller website, all that is really needed is `HTML` and `CSS` as there is not much that is needed. However, larger more complex web pages might start to utilize other languages to store a data and use databases. 

### How Does This All Work? 

![DNS](https://upload.wikimedia.org/wikipedia/commons/7/7e/Dns-rev-1.gif)

Source: Б.Өлзий. (2016, April 14). DNS. Retrieved March 31, 2021, from https://en.wikipedia.org/wiki/File:Dns-rev-1.gif

As you can see from the picture above The DNS act like telephone books for your device. In order this is how the web works: 

1. You connect to the web through an Internet Service Provider or **ISP** and type in a domain address or web address. For example, github.com 
1. Your computer will connect to servers in the network called DNS or **Domain Name Servers**
1. The DNS will communicate with one another and find the IP address that is associated with the domain name that you requested which was (in our example) github.com. **IP addresses are associated with each domain names and are numbers that are up to 12 digits and sepetrated by periods. Example, 192.168.1.0** 
1. Once the DNS gives your computer a unique IP address, your computer will now be able to contact the web server that holds the web page that was requested. 
1. The web server will then send the web page back to your computer.  

# <ins>HTML Structure</ins> #
---

## Understanding HTML Structure, Markup, Tags and Elements 

If you go to any website article, or even an article in a newspaper - You'll understand that the words that need to be portrayed to the reader, must be be organized. Meaning that there is almost always going to be a header that will catch your attention regarding whatever subject, an introduction that will hook you into reading more of the article, and finally the subsections of the article seperated by smaller titles. **HTML** works in a similar if not the same fashion. If you look at the picture below, you can see more of a clearer understanding on how this may look like in **HTML**. 

![HTML Structure](https://3.bp.blogspot.com/-sgm6BBz6KbM/VuarmPKRJ1I/AAAAAAAAG4Q/5GDCRhO09IgiCE2DQXhA0OVaxlylGWvvw/s1600/html-structure.png)

From the very top, the **HTML** _!Doctype_ will be defined to let you know of the type of document. From there as you move down you will see the `<html>` **tag**. Tags are containers (ex. `<hmtl>...</html>`) that will have information in between the opening `<>` and closing `</>` tags. As we move more down on the picture, you may have a clearer understanding. The next **tag** is the `<head>` tag. within a `<head>` tag, it is mostly information for developers regarding the webpage being built. Within this tag, you also include any JavaScript or CSS but we can cover that at a later time. Continuing the explanation of the picture above, the next tag you see is the `<body>` tag. This is the meat of the `<html>` markup. 
Within the `<body>` tag you will see other tags that can determine the size of the lettering - that will be used to explain the heading or title of the webpage, as well as other content like descriptions, or the actual article itself. What is important  is that between the `<body>` tags will display the webpage to the users. **IT IS IMPORTANT THAT EACH TAG HAS AN OPENING AND A CLOSING TAG. `<>` = open `</>` = close**
The following is a code snippet that may help you understand the structure of `<html>`: 

     <!DOCTYPE html>

     <html> 
     
        <head>
        
          <title> This is the title of the page. This can not be seen in the main contents of the page, but can be seen at the top of your browser </title> 
          
        </head> 
        
          <body>
          
            <h1> This is a Header tag. Heading or title is here </h1> 
            
              <p> This is a paragraph tag that can fit an introduction or description or even the main article </p> 
              
            <h2> This can be a sub heading as it is a smaller size header tag. Header tags go to <h6> </h2> 
            
          </body> 
          
      </html>
        
Now that we covered the structure, and the main tags that are used, lets briefly cover the attributes. So what are attributes? Attributes are made up of a name and a value sepaerated by an equals sign, and provide more information regarding the contents of an **element**. An element is what is between the tags. For instance, `<html>` the element is html. So if we include an attribute the element will provide more information. 
As mentioned in an attribute there is an attribute name and a value. The attribute name will indicate what the information is. The value seperated by the equals sign will define or set the information that the attribute name has in store. For example, 

     <p lang="en-us"> This sentence is in English </p> 

The attribute name in this example is "lang" which indicates that a language is used within the element. Then it is seperated by an equals sign to set the value which in this case it is "en-us" and this defines what the language is which is English in this case. 

`<html>` is not really a programming language as it is more of a text markup. Therefore to create an html document you can simply go into your computer and look for notepad or notes and markup the document using `<html>` and as long as you save the document as HTML, this can be used to open up a webpage. 


# <ins>Extra Markup</ins> #
---
`html` has quite the history. There have been multiple versions of `html` but we will cover starting from HTML4. HTML4 was released in 1997. All the elements that were covered in these notes, are available within HTML4. There are other attributes that can be used witth HTML4 which include for example, `<center>` or `<font>`, but these are mostly done with CSS. 
In 1998, XML was released and it was supposed to have new markup languages. Overal, the HTML4 and XML combined in 2000 which created something called **XHTML**. This language basically had more stricter guidlelines compared to the previous versions of HTML. For instance, 
1. every element needs a closing tag except empty elements such as `<img />`
1. attributes names needed to be lowercased
1. depreciated elements were no longer used
1. every element that was opened inside another element needed to be closed in that same element 

---

## HTML Language 
Now that we have briefly discussed some of the history of HTML let us go deeper to try and understand how to write this language. 

Starting with the `<!DOCTYPE>`. What is it? Becuase there are different versions of HTML we need to include which type of HTML we are going to use. With proper declaration of the type of **!DOCTYPE** this will allow the browser to load the contents of the markup correctly. So here is how an html doctype would look as code: 

`<!DOCTYPE html>` 

Now how about if you wanted to make a comment next to some code and not make it part of the code? This is how: 

`<!-- This is a comment -->` 

So now you know clearly how to declare what type of document you will be writing in and also how to make comments. As you recall from previous sections of these notes, you may remember the other elements that we have used thus far. For instance: 

``<head> </head> <body> <h1></h1> <p></p> </body>`` 

With that being said, you can add an **id** attribute to any of these elements. What is an **id** attribute? An id attribute is used to identify an element from other elements that are on your page. This attribute is also known as a **global** attribute because it can be used on any element provided by HTML. 

So how do we use an **id** attribute? the value of the **id** attribute should start with a letter or an underscore and not a number or special character. Each **id** attribute has to be unique so if you want to use more than one you will have to diffrenciate them. Here is an example: 

`<p id="pullquote">...</p>` 

With this attribute you name that element to call that specific element when needed. 
Another attribute that is important to cover is the **class** attribute. This attribute is also used with CSS and will change the style of whatever element uses the same class. 

Here is how you can create and then call a **class** attribute: 

     <html>
         <head>
               <style>             <!-- this is CSS --> 
               
               h1.exampleClass {   <!-- h1 is where the class is and the "exampleClass" is the name of the class --> 
                    color: blue;   <!-- this will make h1 into the color blue --> 
                    }
               </style> 
         </head> 
         <body> 
         
         <h1 class="exampleClass"> EXAMPLE </h1> <!-- the class has been called and the color is blur because it was set from the above CSS -->
         
         </body>
     </html>

Now that we covered some of the attributes, notice how every time you use a `<h1>, <p>` element the browser will start whatever is between those tags on a new line. This is because these elements are known as **block elements**. Another element that are considered block elements is the list elements which is `<ul>` or unordered list (this will display bullet points) and the `<ol>` which is a numbered list. `<li>` is the list elements that will be wrapped around either `<ul>` or `<ol>`. For example, 

     <ul> 
          <li> this is the first bullet point </li>
          <li> this is the second bullet point </li> 
          <li> this is the third bullet point </li> 
     </ul>

Remember that **block elements** start on a new line within the browser. So what are elements that dont start on a new line? This is called **inline elements**. 
You wont always want a new sentence to start on a new line, thus creating the necessity for **inline elements**. Some example inline elements are `<a>` (anchor tags) `<b>` (bold text element) `<em>` (emphasized text) or `<img>` elements. 

So the next you might want to know is how to group all yopur content together. You may want to do this if there is content that need to be in the same space together. Such as a "Home", "About", or "Contact" links. It'll be pretty troublesome if you spread those all out within your web page. To group text and elements together, lets introduce the `<div>` element. 

Inside a `<div>` element you can group together the content you need in the same area so that you can better organize your web page. 
So lets use the example of the list elements and use it with the `<div>` element to group together a list of navigational links that can be used in your web page.

         <div id="header"> <!-- the id attribute is used to attatch an identification to the div element which is called "header" --> 
         
         <ul> 
               <li> <a href="index.html>Home </a> </li>    <!-- you can see that an anchor tag or <a> element is used to internally link the following text -->                        
               <li> <a href="about.html>About </a> </li>
               
               <li> <a href="contact.html>Contact </a> </li> 
         </ul> 
         
         </div> 
         
The following code is all within the header of the webpage as defined by the id attribute. 

Now you know how to group all the contents together and again since this is a **block** the text will start on a new line. So now how about **inline** groupings you may want to include in your webpage? This is when we could use the `<span>` element. The main reason you may find yourself using this element is so you can control the text within the `<span>` element with CSS. Here is an example of how you can use the `<span>` element to keep text all within the same area without starting a new line: 

          <p> this is an <span>example</span> text </p> 
Now that we have the "example" wrapped in `<span>` we can come back with CSS to change only what is wrapped under the `<span>` element while maintaining the grouping of the text without starting a new line. 

Now, if you look thorugh webpages for businesses what you'll notice is a map off to the side or maybe even a dedicated page for a map. How do they do it? of course using this method isn't only for maps, but it kind of gives you an idea of how this element works. The `<iframe>` element will allow you to include a window from another source into your own webpage! 

Another thing to note when using this element is the sizing. So, within the `<iframe>` element you will need to adjust the sizing using the `<width>` `<height>` `<src>` (for the source of the window) and maybe other elements to make your window more friendly such as `<scrolling>` `<frameborder>` and `<seamless>`. An example code snippet of how this may look is like this: 

          <iframe 
               src="https://maps.google.co.uk/maps?q=moma+new+york&amp;output=embed"
               width="450"
               height="350"
               frameborder="0" 
               scrolling="no">
          </iframe> 
    
Last thing, you may want to understand what the `<meta>` is. `<meta>` will most likely be placed within your `<head>` element and is not visible to users. `<meta>` is essentially the description of your webpage and will provide information such as the description,  any keywords for the search engine, robots, the author of the webpage, a pragma or caching page, and the expiration of cache. 

# <ins>HTML5 Layout</ins> #
---
Up until now, traditional HTML has been covered. As mentioned before regarding the history of HTML, there exists one more version of HTML that is currently in the process of being fully updated. This is HTML5. Starting with the layout, with traditional HTML web developers use the `<div>` elements to create the structure of the page. HTML5 introduces a new set of elements that will allow developers to divide up the parts of the webpage. 

### Headers and Footers 

Starting with the headers and footers ( `<header>` `<footer>` ), in HTML5 the `<header>` element is placed on the top of the page and can include the site name and the main navigations such as the "home", "about", or "contact" navigational links you may find on most webpages. The `<footer>` will contain the copyright information you might've seen on some webpages in small text. This is an example of how the `<header>` and `<footer>` is used: 

          <header>
               <h1> This can be the title displayed to users </h1> 
               <nav> 
                    <ul> 
                         <li><a href="" class ="current"> Home</a> </li> 
                         <li><a href=""> About </a></li> 
                         <li><a href=""> Contact Us </a></li> 
                    </ul> 
               </nav> 
          </header> 
          <Footer> CopyRight 2021 </footer> 
### Navigation 

In HTML5 the `<nav>` element (as seen in the example above) is used to wrap the navigation block for site navigation. 

### Articles 

The `<article>` element is used to house articles, blogs, forum posts, comments, piece of independent content. `<article>` elements can also have their own `<header>` and `<footer>` elements. Let'e take a look at a snippet of how `<article>` elements are used: 

          <article> 
               <figure> 
                    <img src="images/example.jpg" alt="example" />   <!-- The image and its caption all within the article --> 
                    <figurecaption> Example </figcaption> 
               </figure> 
                    <hgroup> 
                       <h2>Example #1 <h2>                <!-- Our heading groups --> 
                       <h3>Example #2 </h3> 
                    </hgroup> 
                        <p> This is an example paragraph inside of an article! </p> 
           </article> 
This is one grouping for an article for one subject. 

### Asides 

An `<aside>` element has two purposes that depend on whether it is nested in between an `<article>` or not. If the `<aside>` element is nested in between an `<article>` element, then it will contain information regarding that article. If the `<aside>` element is used outside of the `<article>` element, than whatever is nested in between the `<aside>` element will contain information related to the site itself. Let's take a look at how the `<aside>` element is used outside of an `<article>`:

               <aside>
                    <section class="example1"> 
                         <h2>Example 1</h2> 
                         <a href=""> This can be an example for example 1</a> 
                    </section> 
                    <section class="example2"> 
                         <h2>Example 2</h2> 
                         <a href=""> This can be an example for example 2 </a> 
                    </section> 
               <aside> 
               
### Sections 

As seen in the above code snippet, a `<section>` element will group related content together. **typically each section will have its own heading**. One thing that should be notes is that the `<section>` element should not be used to wrap the entire page with - unless the web page only has that one peice of content. 

### Heading Groups 

As seen in the code snippet from the `<articles>` section, you'll notice something that looks like this: `<hgroup>`. As mentioned in the comments, this is a heading group. This element will group together any of the 6 <h> elements that is more than 1. With this element you can create a title within an element and then a subtitle within an element. 
     
### Figures 

Again using the example code snippet from the `<article>` section you will also notice something that looks like this: `<figure>` and `<figcaption>`. These elements can be used to contain any content that is referenced from the main flow. These elements does allow use of a wide variety of content and not just images. For instance you can provide, images, videos, grpahs, diagrams, code samples, or even just text. `<figure>` is the content and the `<figurecaption>` as the name suggests is the caption for that content. 

### Sectioning Elements 

Just because HTML5 is newer than the traditional HTML, does not mean we abandon all the old ways. In HTML5 we can use `<div>` elements once again to group together related elements. 

### Linking Around Block-Level Elements 

The `<a>` element or the anchor tag, is also still used within HTML5 and can be used to make an entire block into a link. 

### Compatability With Older Browsers 

HTML5 is still relatively new. Therefore, there will be some browsers that still can not understand HTML5. However, there is still a solution. What you can do to make older browsers understand HMTL5 if include a snippet of CSS that will render neww elements into block-level elements. Furthermore to style using CSS on older browser you need to include JavaScript which is known as **HTML5 shiv** or **HTML5 shim**. 

# <ins>Process and Design</ins> # 


