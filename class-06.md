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
