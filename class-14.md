# What Google Learned From its Quest to Build the Perfect Team /CSS # 

Article Author: Charles Duhigg
Date published: Feb 25, 2016 
link: https://www.nytimes.com/2016/02/28/magazine/what-google-learned-from-its-quest-to-build-the-perfect-team.html

After changing her paths to something more exciting, Julia Rozovsky, went to a business school in Yale School of Management. While she was attending, she was placed in a study that was engineered by the school to create tighter bonds within the group. Groups are very common when it comes to many M.B.A programs, but it is only becasue groups are a necessity in the chaotic real world. Essentially, by creating a tight group, people in the group will start to synchronize and more-easily share the information they possess and communicate more effectively. Google, understood the real need for team building and also came up with some data involving a boost in productivity. 

# CSS # 
## Transforms ## 
There is another way to size, position, and change elsments. This is by using the `transform` property. This is how it may look like in code: 

          div {
              -webkit-transform: scale(1.5);
                 -moz-transform: scale(1.5);
                   -o-transform: scale(1.5);
                      transform: scale(1.5);
            }
      Source: https://learn.shayhowe.com/advanced-html-css/css-transforms/
      
      
The transform property is able to change elements within two-dimensions or three-dimensional panes. The Two-dimensional transforms use the x and the y axis, and the three-dimensional transforms will work on the x axis, y axis, and the z axis. There are a lot of values that can be passed through the two-dimensional, and the three-dimensional. Here is a list of all the 2d tranform values. 
  * 2D rotate 
  * 2D scale 
  * 2D Translate
  * 2D skew 
  * 2D cube 

This is a list for the 3D values: 
   * 3D rotate
   * 3D scale 
   * 3D Translate
   * 3D skew


## Transitions and Animations ## 
Transition is a property that will change the state of the element. For instance, change the color of a background upon mouse hover. Here is a code snippet of what it may look like in code: 

              .box {
                  background: #2db34a;
                  border-radius: 6px
                  transition-property: background, border-radius;
                  transition-duration: 1s;
                  transition-timing-function: linear;
                }
                .box:hover {
                  background: #ff7b29;
                  border-radius: 50%;
                }
            Source: https://learn.shayhowe.com/advanced-html-css/transitions-animations/
            
            
 These are the transition properties: 
      
      * background-color
      * background-position
      * border-color
      * border-width
      * border-spacing
      * bottom
      * clip
      * color
      * crop
      * font-size
      * font-weight
      * height
      * left
      * letter-spacing
      * line-height
      * margin
      * max-height
      * max-width
      * min-height
      * min-width
      * opacity
      * outline-color
      * outline-off
      * setoutline-width
      * padding
      * right
      * text-indent
      * text-shadow
      * topvertical-align
      * visibility
      * width
      * word-spacing
      * z-index

      Source: https://learn.shayhowe.com/advanced-html-css/transitions-animations/
      
  
