# Error Handling and Debugging # 
Unless you are a prodigy programmer, you will not have perfect code. Don't worry, I believe that errors in code is just something that is going to happen as long as you write code. Fortunately, you and I won't be the only ones making these errors in code. That is ultimately why debugging exists along with many other tools that can help developers find these errors - and be able to turn in code that seem like it was flawless from the start. 
A lot of the times as I have experienced already, I will make errors in code and wont be able to find the error. This is another reason why you should read your code line by line or in bigger cases, functions and methods at a time to help track the error. 
You should also try and understand the **order of execution** so you can understand what is out of place and track down errors in code more efficiently. Try to visualize, how you want your code to work (to better understand the order of execution). Let's say you want to greet a user. To do this in a simple way you can think of something that can ask for an input value. Then hold the input value. Then output the input value with a greeting message. That was more generalized, but essentially the order of how you can code. 
Just like how we should read code line by line to understand our own code to prevent problems, the interpreter will also read the code line by line and output an error if there is one. Thankfully that feature exists, otherwise you would spend alot of time looking at your screen trying to figure out where you went wrong. 
## Execution Context and Hoisting ## 
There are generally two phases of activity that occurs when the code you write executes. The first phase is the preperation phase where declare all the variables and create functions and arguments. Then there is the execution phase where now that code can assign values to varibales and reference functions and so on. 
A concept called **hoisting** is used or is defined when you are able to call a function before they have been declared. That is because the preperation is completed within context of the called function. For instance: 
        
        var example = exampleFunction();
        function getexample() {
          function exampleFuction() {
          
In this example, you can see that the exampleFunction is used or nested in the getExample function. The first line of code will not work because of this. Here is something that might actually work: 

      var example = exampleFunction();
      function exampleFunction() { 
      
The exampleFunction in this instance would work because it is within the context of the function being made. 

## Debugging Workflow ## 
There are many tools within browsers that will help you catch errors within the developer tools if you right click and hit inspect, or if you simply press f12. Almost every browser people use today will have this feature. A good habit to form while writing code is to use the console.log. This can help you track and see if the code you wrote before you console.log is returning the expected value. You can check this on the web developer tools in the browsers. This is a good way of understanding where you went wrong through constantly checking on the console log. 
There are other tools you can use to find errors in the developer tools such as the step through. This tool will give you the oprtion to pause the page while it is loading and to see any error that take place in live time. 

## Handling Exceptions ## 
As a developer you can also expect some code to fail, but as long as that code is working to get to your objective you can use some handling exception keys like **try**, **catch** and **finally**. How you can use these is by entering code you think might fail or throw an exception under the try. If there is an error it will go to the next block which is catch. Under catch, you can set up another code block to try and fix that exception that the code under try is throwing. The last one, or finally. The code that is under finally will run regardless if it failed or suceeded. 
You can also generate your own errors so that you can beat the race against your opponent, the code editor. You might want to make your own errors so that the code will not cause errors further down the line as you write more code. 
To generate an error the keyword is `throw new Error()`. 

In general, you should take the most precaution so that you can try and prevent errors in code before. With the tools available to us all, we can do a lot to prevent errors in code. We have tools like the web developer tool in our browsers, we can use codeing playgrounds to make sure a block of code even runs, we have other resources such as Google.
The best method is to understand what an error is, and to go through code line by line and understand why the error is happening - so that you can find a better solution. 
