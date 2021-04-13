# Domain Modeling # 

Domain modeling is essentially the translation of the real world into code. Replicating the real world using code that will represent anything that has to do with an object from the real world. 

## Domain Modeling Example ## 
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
                             
To name your rows or columns you can simply add the `<th>` inside the `<tr>`. You determine to label either the row or column by including the scope attribute. So, within the `<th>` you would add `scope="row"`to label a row, and `scope="col"` to label a column. 
 
## Spanning Columns ## 
