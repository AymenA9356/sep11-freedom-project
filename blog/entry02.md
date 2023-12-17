# Entry 2
##### 12/11/2023

# Navigating the jQuery Jungle: A Developer's Journey through Problem Solving

## Introduction
Welcome to a developer's adventure in the world of jQuery! In this blog, we'll explore some common problems faced while working with jQuery and delve into the creative solutions that helped me overcome them. jQuery, a fast and concise JavaScript library, has been a go-to tool for many developers seeking to simplify client-side scripting. Let's dive into the challenges and solutions encountered along the way.

## Challenge 1: Unresponsive Event Handling
One of the initial challenges I faced was making sure that event handlers were responsive, especially when dynamically adding or removing elements from the DOM. jQuery's `.on()` method came to the rescue. This versatile method allowed me to attach event handlers to elements, even those created dynamically, ensuring a consistent and responsive user experience.

```javascript
// Example: Dynamically added element
$(document).on('click', '.dynamic-element', function() {
    // Your event handling code here
});
```

Solution:
Use event delegation by attaching the event handler to a parent element that exists in the DOM when the page loads. This ensures that events are captured for dynamically added elements.



## Challenge 2: Cross-browser Compatibility

Issue: Ensuring consistent functionality across different browsers.

Solution: Use the `.ready()` method to ensure that your code executes only when the DOM is fully loaded. This helps avoid cross-browser inconsistencies related to the timing of script execution.
```javascript
// Ensuring cross-browser compatibility with .ready()
$(document).ready(function() {
    // Your code here
});
```

Starting a journey with jQuery has proven to be a wonderful and hard experience. My ability to solve problems creatively and in combination with the library's capabilities has allowed me to create online apps that are cross-browser compatible, responsive, and efficient. As the field of development changes, jQuery remains a useful resource in my arsenal.


## Skills
During this process, I developed the ability to on **How to learn**. I gained a lot of knowledge in Javascript that I never would have imagined. I'm getting closer to developing my Airplane calculator thanks to this. Another skill I learned was **Time management**. Time management is very important. By incorporating these strategies, I can effectively prioritize tasks, create a development roadmap, and work towards building a successful MVP using jQuery


## EDP
Currently, we are in the second part of the EDP (Engineering Design Process) which is researching the problem. Now that we know and defined the problem we can now search about the problem. In the world of flight simulation, many planes only give you the actual numbers for your take-off speeds. But the plane's computer does not know if the runway is wet, dry, or icy. So I am creating a calculator that will take all of those factors into account like wind speed and direction, runway condition, temperature, and air pressure.



[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)