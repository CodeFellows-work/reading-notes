# JavaScript Objects # 

## What is an Object? ## 
Objects are essentially a group of variables and functions put into an object as properties of that object. In an object, those functions stored are known as methods. 

So for example if you had an object for a car, you would have the main car object, then inside the car object, you have information about the car or varibales for info on the car. The variables are known as properties of the car. Then, if you have a function in your object, that is known as a method. 
    
          // MY OBJECT
          const car = { 
          // MY OBJECT PROPERTIES 
          name= 'BMW', 
          doors= '4',
          driveType: ['AWD', 'FWD', 'RWD'], 
          availability= true; 
          // OBJECT METHODS
          selectCarForTestDrive: function(){ 
              alert("you have selected the ${car.name} to the list); 
              return this.availability = false; 
              } 
          } 
          
### Object Notations ### 
* Literal Notation


The **Literal Notation** is easy to use and one of the most popular ways to create object. You start of by decalring an object just like you would with variables. And then you use `=` followed by a `{`. Inside these curly braces you store the objects properties, or variables and values that make up the object. You include a function in the object and the function will become a method. This is how the code may look like: 

            const myDog = { 
            // the properties of the object
            name: 'Buddy',                         
            'favorite toys':[rubber ducky, sticks], 
           
           //the method in the object 
           callTheDog: function(){
           console.log('Come here' ${name};
           } 
* Dot notation 
The Dot notation is used to access the properties of the object or the method in the object. You can also access properties with square brackets. 

            // here I console log the name of the myDog object. 
            conole.log(myDog.name); 
            
            // to use square brackets I can put the variable inside of the square brackets. 
            console.log(myDog['example name'] 
            
## JavaScript DOM ## 
The **Document Object Model** or DOM, is used to access HTML elements with JavaScript. Using this model, you can also add elements to HTML. Some methods you can use with DOM include: 

* getElementById 
This selects the element with an id from JavaScript 

* querySelector 
This selects the css selector from JavaScript 

* getElementsByClassName
This selects the element with the class name for that value 

* getElementByTagName 
This selects the element on the page with what the tag name is set to 

* querySelectorAll 
This selects one or more css selcetors that will match 
            
## Previous and Next Sibling ## 
To select and access your previous sibling we need to understand where are starting position is. We call the ElementById and set the value of our starting point, and then we can use our previous sibling. When we select our previous sibling, we will need to start with the starting point and go backwards which will be our previous sibling. The same concept goes for our next sibling. The starting point will dictate what the next sibling would be. This is an example code: 

        // let's say we have an <ul> and have many <li> 
        
        <ul> 
            <li id="example1"> 1</li> 
            <li id="example2"> 2</li> 
            <li id="example3"> 3</li> 
       </ul> 
 So we want to call the previous but first we have to set the starting point. I am going to choose `id="example2"` as my starting point. 
        
        let exampleStart = document.getElementById('example2'); 
        
        //now I can get the previous sibling or the next. 
        
        let examplePre = exampleStart.previousSibling; // this will store example1 from exampleStart in examplePre 
        
        let exampleNext = exampleStart.nextSibling; // this will store example3 from exampleStart in exampleNext 
  
 ## First and Last Child ## 
We can find first child and last child with the same concept of determining the starting point. So in our example we used an <ul> and nested <li> x 3 into it. We then got the previous child and the next child by determining the starting point. This time, we will set the starting point within the main element which is <ul> to essentially order the <li>. So once you stated that the <ul> us our starting point, you can then determine the first child within it or the last child. This is how it may look in code: 
    
           // this statement will assign the <ul> first index of it as the starting point, which would be <li id="example1"> </li> 
          let exampleStart = document.getElementById('ul')[0] 
          //now we can get the first child 
          let exampleFirst = exampleStart.firstChild; 
          //The last child 
          let exampleLast = exampleStart.lastChild; 
          
We can also use node values to pick a value that may be next to another value within an element.

## innerHTML ## 
So, there are mutiple ways your JavScript can access the HTML. A property that can be used id `innerHTML` . The innerHTML node can be used on any element node, meaning the text content and not what stores the text content. 

    // So let's use the same example as from before but this time use a innerHTML.
           <ul> 
            <li id="example1"> 1</li> 
            <li id="example2"> 2</li> 
            <li id="example3"> 3</li> 
       </ul> 
       
       // this will output what is inside of example 1. 
       let getContent = document.getElementById='example1'.innerHTML; 
 
