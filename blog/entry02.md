# Entry 2
##### 12/11/2023

# Navigating jQuery

## Introduction
In this blog, I'll discuss some issues I ran into when using jQuery and the way that I was able to fix them. Many people have turned to jQuery, it is a quick and easy-to-use JavaScript library when they want to make client-side scripting simpler.

## Challenge 1: Unresponsive Event Handling
One of the initial challenges I faced was making sure that event handlers were responsive, especially when dynamically adding or removing elements from the DOM. In jQuery's [documentation](https://api.jquery.com/on/) the  `.on()` method came to the rescue. This versatile method allowed me to attach event handlers to elements, even those created dynamically, ensuring a consistent and responsive user experience. For example:
``` js
$( "p" ).on( "myCustomEvent", function( event, myName ) {
  $( this ).text( myName + ", hi there!" );
  $( "span" )
    .stop()
    .css( "opacity", 1 )
    .text( "myName = " + myName )
    .fadeIn( 30 )
    .fadeOut( 1000 );
});

```
 So let's break this down. So the first line is turning on/running an event called `myCustomEvent` this is followed by a function. Not sure what `this` is used for but I think that it is saying that the particular code should run. Then we can see that the name is followed by a string `", hi there!". The rest of the code is just a way for the name to just start fading in and out.

```javascript
// Example: Dynamically added element
$(document).on('click', '.dynamic-element', function() {
    // Your event handling code here
});
```

Solution:
Use event delegation by attaching the event handler to a parent element that exists in the DOM when the page loads. This ensures that events are captured for dynamically added elements.



## Challenge 2: Cross-browser Compatibility

 Another issuse I was having was Ensuring  the consistent functionality across different browsers.

The way I solved this way by using the `.ready()` method found [here](https://api.jquery.com/ready/) this ensures that your code executes only when the DOM is fully loaded. This helps avoid cross-browser inconsistencies related to the timing of script execution.
```javascript
// Ensuring cross-browser compatibility with .ready()
$(document).ready(function() {
    // Your code here
});
```

This journey with jQuery has proven to be hard procces, And my ability to solve problems with the library's capabilities has allowed me to create compatible, responsive, and efficient. As the of development changes, jQuery remains a useful resource in my tool belt.


## Skills
During this process, I developed the ability to on **How to learn**. I gained a lot of knowledge in Javascript that I never would have imagined. I'm getting closer to developing my Airplane calculator thanks to this. Another skill I learned was **Time management**. Time management is very important. By incorporating these strategies, I can effectively prioritize tasks, create a development roadmap, and work towards building a successful MVP using jQuery


## EDP
Currently, we are in the second part of the EDP (Engineering Design Process) which is researching the problem. Now that we know and defined the problem we can now search about the problem. In the world of flight simulation, many planes only give you the actual numbers for your take-off speeds. But the plane's computer does not know if the runway is wet, dry, or icy. So I am creating a calculator that will take all of those factors into account like wind speed and direction, runway condition, temperature, and air pressure.



[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)