# Forms and JS Events # 
## Forms ## 
Forms on web pages are a good way to get feedback and improve the business operations as a whole. Forms can be used in different ways as well - not just for business needs. For instance, you can use a form to search the web. If your wondering what that means, when you Google things, you are using a form. Your inputting some kind of data that will present you with its findings or in turn an action happens from a result of you enetering information. 
### Form Controls ### 
So, what are the different types of forms you may have encountered? There are a few: 
  * Adding text like your name or password 
  * making choices through use of radio buttons or a checkbox 
  * text area to maybe leave some feadback 
  * a drop down menu for you to choose from 
  * upload files or download files through a button 
  * and finally, the submit button 
### Form Operation ### 
Now, we kind of understand what a form may look like, and maybe even know why its there on a web page. But how do forms actually work? 
1. You start with information. You enter data into a form box - whatever it may ask you. Then you click submit and it sends the data. 
2. that information is sent to a server. 
3. The server will process that information that has been inputted with a hgih-leveled programming language and even can be sent to a database. 
4. Whether the information is stored or processed, you can expect to find another page informing you that the your sata has been submitted. That is the server sending you back another page. 
## Parts of a Form ##
To start off, even a form has structure. You will use a `<form>` tag to indicate that you will use a form. Within the form tag there are attributes that will follow. `<action>` attributes will always follow the <form> tag and is the link that will be the form. So now the code will resemble this: 
  
      <form action ="link to form"
      
But there is another attribute you will use to complete this element. It is the method attribute. The method attribute will have two options. THe "get" and the "post". It is recommended to use the get in the method when you are utilizing smaller forms. The get method will just tack on the values from the form and added to the end of the URL of your form to send to the server. 
The post method is recommended for bigger forms. This method will send to the server the HTTP headers.
### Text Input ### 
A lot of forms will have text input to retrieve from the users. For you to get input you use the `<input>` element to start. Within the <input element you will set the attributes by using `type = "text"` to clarify that you want a text input. Forms are all about values, so you also have a name attribute that it will store. You can also set the size of the text input by using size. Finally you can set how biug the text input would be by using "maxlength". 
Text input is not only for names but passwords. You use the `<type = "password` to define to the form that your entering a pasword. This will turn your text into black dots so that you dont see what your typing. 
How about if you want a text box? And this can be for personal feedback from a user. You use the `<textarea>` element to place a text box. 

### Options ### 
You may have already realized, but a lot of forms on the Internet will also have options for you to choose from. This can be either in a radio button form, which looks like bullet points you can click on, check boxes - which allow you to check each box for a multiple answer input a drop down list box, or a multiple select box. 

This is how all of those look in code: 

Radio Button
      
      <input type="radio" name="sunny" value = "value sent to server for chosen option" checked = "checked" /> 

Chckboxes 
    
      <input type="checkbox" name="sunny" value="value sent to server" chcecked="checked"/> 
      
Drop Down List box 

    <select name ="the category for the box"> 
        <option value="an option for that category> The option </option> 
        ...
     </select> 
     
Multiple Select Box 

    <select name="category" /> 
      <multiple="multiple options">
        <option value ='an option for that category'>The option</option> 
        </select> 
        
### More on <input> ### 
With the `<input>` element you can also make an input box. This is used so that users can upload files. This input can be seen a lot in educational web pages, for you to perhaps turn in an assignment. 

    <input type="file" 
    
You can also use the <input> element to create a submit button. 
  
    <input type="submit" 
    
More on the submit button, you can make your submit button more fancy by using an image as the submit button. 

    <input type=ïmage" 
    
To simply create a button that does not submit your data (maybe it can) but maybe you want to use this button for other things like to add to bookmark within a page. You can use the button element

    <button> 
    
### Labeling Your Form ### 
Now, you have the ability to make a text input, some yes or no options, a multiple answer form, and be able to submit. But none of that really matters because no one will know what the form is for, or what kind of data to use when inputting. That is why we label. You can use the `<labnll>` element to make labels around your input forms to let your user know what to enter. 

### Grouping ### 
How about making a form that asks for your name, address, and phone number. If you think that is creapy, you probably should remember when you filled out your information on Amazon. Now it does'nt sound as creapy? Well you can make forms that are bundled together using the `<fieldset>` element and the `<legend>` element. The <fieldset> where the forms will be at. The <legend> just like the name implies, gives you the idea of the form and it is a label regarding the form. 
  
# List, Tables, Forms # 

