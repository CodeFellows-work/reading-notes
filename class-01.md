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

From the very top, the **HTML** _!Doctype_ will be defined to let you know of the type of document. From there as you move down you will see the `<html>` **tag**. Tags are containers (ex. `<hmtl>...</html>` that will have information in between the opening `<>` and closing `</>` tags. As we move more down on the picture, you may have a clearer understanding. The next **tag** is the `<head>` tag. within a `<head>` tag, it is mostly information for developers regarding the webpage being built. Within this tag, you also include any JavaScript or CSS but we can cover that at a later time. Continuing the explanation of the picture above, the next tag you see is the `<body>` tag. This is the meat of the `<html>` markup. 
Within the `<body>` tag you will see other tags that can determine the size of the lettering - that will be used to explain the heading or title of the webpage, as well as other content like descriptions, or the actual article itself. What is important  is that between the `<body>` tags will display the webpage to the users. **IT IS IMPORTANT THAT EACH TAG HAS AN OPENING AND A CLOSING TAG. `<>` = open `</>` = close**
The following is a code snippet that may help you understand the structure of `<html>`: 

`<!DOCTYPE html>

     <html> 
     
        <head> </head> 
        
          <body>
          
            <h1> This is a Header tag. Heading or title is here </h1> 
            
              <p> This is a paragraph tag that can fit an introduction or description or even the main article </p> 
              
            <h2> This can be a sub heading as it is a smaller size header tag. Header tags go to <h6> </h2> 
            
          </body> 
          
      </html>`
        
            










