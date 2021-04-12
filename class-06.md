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
            

      
