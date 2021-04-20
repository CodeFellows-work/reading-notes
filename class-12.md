# Chart.js And Canvas #
## Chart.js ## 
From previous notes, we understood how to make tables, and why they might be important. To have a little refresher on the importance of tables, think about schedules, and data. A chart is similar to a table in the way that data is used to create a method for users to see the compilation of the data in one place. Charts, are an excellenet tool to compile data and showcase the data. 
So to start using charts, you will need to get on your terminal to and use `npm install chart.js`. This is a JavaScript plug in that uses an HTML canvas to draw essentially a graph that can display your compiled data. 
So after you have properly installed the chart, you can move onto the next step which would be to start drawing the chart. Add this to your HTML. 
  
      <canvas id='buyers' width='600' height='400'></canvas> 
      
You do not need to use the specified hight and width displayed in this example. So now that you have added the element with its attributes to your HTML, you will need to add a script tag with the following: 

      <script> 
        var buyers = documnet.getElementById('buyers').getContext('2d) 
        new Chart(Buyers).Line(buyerData);
      </script> 
      
      Example is shown on this website: (https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/) 
      
So now you have incorperated this script tag in your HTMl, you will now need to enter some data within the script tag. The example shown on the site shows this: 
      
       var buyerData = { 
           labels: ["January" , "Febuarary", "March", "April", "May", "June"], 
           datasets: [
                { 
                  fillColor: "rgba(172, 195, 132,0.4)", 
                  strokeColor: "#ACC26D",
                  pointColor: "fff", 
                  pointStrokeColor: "#9DB86D",
                  data: [203,156,99,251,305,247]
                 }
               ]
             }
             
             This is a line chart 
             Source: https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/
             
             
With this charts plug-in, you are not limited to only a line chart and you can use a pie chart, or a bar chart as well. What I notice regarding this code, is that - it looks like CSS and JavaScript are combined. 

## Canvas ## 
### Basics ### 
We are intoducing a new element which we have not covered yet which is the `<canvas>` element. The <canvas> element will take in two attributes which is the width and height. Ofcourse this is also optional and can also be set using the DOM properties. If you choose not to use the Width and the Height attributes, the defualt will be 300px wide and 150px high. As a matter of fact, this element can also take in most attributes that a normal img element can use such as margin, borfer, and picture. This is an example of where the <canvas> element is used: 
      
                        <!DOCTYPE html>
                        <html>
                        <head>
                        <meta charset="utf-8"/>
                         <title>Canvas tutorial</title>
                         <script type="text/javascript">
                          function draw() {
                            var canvas = document.getElementById('tutorial');
                            if (canvas.getContext) {
                              var ctx = canvas.getContext('2d');
                              }
                            }
                        </script>
                        <style type="text/css">
                          canvas { border: 1px solid black; }
                        </style>
                        </head>
                        <body onload="draw();">
                       <canvas id="tutorial" width="150" height="150"></canvas>
                        </body>
                        </html>
                        
                        Source: https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage
                        
### Shapes with Canvas ### 
An intersting feature that the canvas element provides you with is the ability to make shapes. Canvas uses lines to path its way into a shape. For instance: 

        fillRect(x, y, width, height)
        
        this will draw a rectangle
        source: https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes        
A functionA you should start to use with the <canvas> element to draw lines or **paths** are these functions: 
  * beginPath()
Then there are the methods:
  * closePath()
  * stroke()
  * fill() 

### Colors ### 
The <canvas> element also can be colored. You use these properties to set them: 
  * fillstyle = color 
  * strokeStyle = color

For a transparent look you use: 
* globalAlpha = transparencyValue 

### Drawing text ### 
On a final note, you can choose to draw your text using some methods such as: 
  * fillText(text, x,y, [, maxWidth]) 
  * strokeText(text, x, y [, maxWidth])
