# Domain Modeling # 

Domain modeling is essentially the translation of the real world into code. Replicating the real world using code that will represent anything that has to do with an object from the real world. 

## Domain Modeling Example ## 

### Figure 1 ### 
![Domain Modeling](https://miro.medium.com/max/700/1*kM41O4gBK3BvXI0870A_kA.jpeg)

Source: Chursin, O. (2017, December 27). A brief introduction to domain modeling. Retrieved April 13, 2021, from https://olegchursin.medium.com/a-brief-introduction-to-domain-modeling-862a30b38353

# Tables # 
A table will represent your data in an organized fashion so that anyone can interpret data points and understand trends as well as comparisons. A table can be useful in your web page for instance, you can use a table element to create a calander for a dental web page to schedule your appointments. To use the table element you will use `<table>`. Within `<table>` just like how `<li>` is nested inside `<ul>`, you use `<tr>` to indicate a new row, and within that you nest the `<td>` to indicate a new cell. 

    <table> 
      <tr> 
        <td> example data </td> 
        <td> example data </td> 
      </tr> 
     </table> 
     
     This will output as :   | example data |  example data |
                             |--------------|---------------|
                             
To name your rows or columns you can simply add the `<th>` inside the `<tr>`. You determine to label either the row or column by including the scope attribute. So, within the `<th>` you would add `scope="row"` to label a row, and `scope="col"` to label a column. 
 
## Spanning Columns ## 
There are also times where you will need to stretch out some rows, so that it can go up to a certain column. You might see this kind of spanning in job work schedules, or class schedules for school. So to put what I just said into perspective, these are the tables that you might need to create: 

### Figure 2 ###
![Spanning Columns](https://www.brainbell.com/tutorials/HTML_and_CSS/images/0131855867/graphics/04fig12.gif;423381)

Source: BrainBell. (2016, August 01). Spanning columns. Retrieved April 13, 2021, from https://www.brainbell.com/tutorials/HTML_and_CSS/Spanning_Columns.htm

As seen in figure 2, you can see that the header covers the first two columns. This is spanning columns. To use this attribute, you just need to add `colspan = "whatever number"` you can add this attribute into wither the `<tr>` or the `<td>` to where you want the span happening within a table. 

## Long Tables ## 
If you happen to have a lot of data, there is another element for that, which can help you sort large amounts into a big table. Within this table, just think of another HTML document build within HTML. What I mean by this is that this table will have an element for a head, body, and a footer. So to start off making the table, under the `<table>` element, the `<thead>`. This element will hold the header of your table and is most likely your table labels for columns. 
After the `<thead>` element is closed, you will move on to the main portion of your table with `<tbody>`. This element is like all the content or data you will put into your table. Finally, you use the `<tfoot>` element to add the footer of your table - and this can be things like totals.

## Old code table Styling ## 
To create kind of a styling to your tables you can use the width and spacing attributes to create gaps in bewtween each row and column. You can also use border attributes to create a border on your table or between rows and columns. 

# Object-Oriented Programming # 
Somewhat continuing off of **Domain Modeling**, a common thing to do is use a **constructor notation** to create a new object. To do this you declare a variable (such as using const, let, var) with your objects name. Then you use "=" followed by the `new` keyword and the object constructor, to create a new object. This creates an empty objects which then you can add things to. 

         const hotel = new object() {
         hotel.name = 'Hilton Suites'; 
         hotel.rooms = 300;                 // properties 
         hotel.booked = 150; 
         
         hotel.checkedAvailable = function() {
            return this.room - this.booked;         // method
            } 

You can update the property values with an assignment operator (=) by calling the object followed by a period, then the property you want to update followed by the assignment operator, then the value. You can also use square brackets to update the value. If you want to delete a value you can use the `delete` keyword that will be placed in-front of the object, to delete the objects value or clear the string. 

        hotel.name = "whatever name" // to update a property value 
        
        hotel['whatever name'] = 'park' // to update the property
        
        delete hotel.name; // to delete the property name 
        
        hotel.name = ''; // to clear the string 

Another thing to note is that within the constructor notation, you can add several properties at once. You can do this by running the property perameters through the object. Then you can you the `this` keyword to assign property values. 
        
        function hotel(name, rooms, booked) { 
        this.name =name; 
        this.rooms = rooms;
        this.booked = booked; 
        
You can also create arguemnents for an object that will have all the proerty values
        
        const hotelOne = new Hotel('Hilton1', 200, 180); 
        
        // hotelOne has the arguements of Hilton 1 name, 200 rooms, and 180 booked
        
## Array Objects ## 
Arrays are actually objects as well. It is a type of object that cna hold a related set of information. Another difference an array has with other objects is the way you call a value. You use indexes in an array to specify a value. 

## Built-in Objects ## 
What are built-in objects? These are objects that are provided by JavaScript. There are generally three types. 
1. Browser Object Model 
2. Document Object Model 
3. Global JavaScript Objects 
