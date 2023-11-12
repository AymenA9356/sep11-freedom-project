# Deciding on my tool
##### 11/06/2023

# Embarking on the Freedom Project Journey with jQuery

## Overview

In the inaugural entry of the Freedom Project (FP), I am thrilled to share my decision to utilize jQuery as the primary tool for this exciting endeavor. This entry will delve into the rationale behind choosing jQuery, the initial steps of tinkering with it through code, and what I envision creating with this powerful library.

## Tool Selection

After careful consideration and evaluation of various options, I have chosen jQuery as the cornerstone for my Freedom Project. jQuery's widespread use, simplicity, and versatility make it an ideal candidate for the dynamic and interactive aspects of my project.

## Why jQuery?

1. **Community Support:** jQuery is a widely adopted JavaScript library, ensuring broad community support and an abundance of resources. Its popularity is indicative of its reliability and suitability for a variety of projects.

2. **It is easy to use:** jQuery simplifies complex JavaScript tasks, offering a more concise syntax for common actions. This ease of use accelerates development and reduces the learning curve, making it an excellent choice for projects with tight timelines.

3. **Compatibility:** jQuery is designed to work seamlessly across different browsers, addressing potential compatibility issues that can arise in web development projects.

## Tinkering with jQuery (Code)

To acclimate myself to jQuery, I have begun experimenting with its syntax and functionalities. Using the help of the [jQuery Website](https://jquery.com/), [jQuery Documentation](https://api.jquery.com/), and the [jQuery Learning Center](https://learn.jquery.com/) I was able to make a webpage with a button and a paragraph, When the button is clicked, change the text of the paragraph to a predefined message. but the problem is that I do not know how to do that so I did what any person would do and searched it up in jQuery documents. The first thing I did was import a CDN into [jsbin](https://jsbin.com/?html,output). I then used my prior knowledge of HTML and made a button and a paragraph using the lorem Ipsum which is placeholder text. In the javascript file, I used the code `$(document).ready(function()` the `$(document)` Selects the document object, and the `.ready()` Attaches a function to be executed when the document is fully loaded.  I then used `$(document).ready(function(){...})` to ensure that the jQuery code inside the function is executed only when the document is fully loaded. `$("#changeTextButton").click(function(){...})` This sets up an event listener for the click event on the button with the id "changeTextButton." `$("#outputText").text("New Text!");` his changes the text content of the paragraph with the id "outputText" to "New Text!".This example shows how to use jQuery in a simple way to manage user interactions and dynamically change webpage content. Full Code:

HTML
```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Change Text Example</title>
    <script src="https://code.jquery.com/jquery-3.6.4.min.js"></script>
</head>
<body>

    <button id="changeTextButton">Change Text</button>
    <p id="outputText">Original Text</p>

    <!-- Your other HTML content goes here -->

    <script src="app.js"></script>
</body>
</html>
```
Javascript
``` js
$(document).ready(function(){
    // Code to run when the document is ready

    // Event listener for the button click
    $("#changeTextButton").click(function(){
        // Change the text of the paragraph
        $("#outputText").text("New Text!");
    });
});
```

## Skills
One skill I learned during this process was **how to learn**. I learned a lot of things that I thought I would never learn in Java script. This brings me closer and closer to coding my Airplane calculator. Another skill I learned was **How to read**, If I did not read the documentation and learn and understand it properly I don't think I would be able to do this. Mini coding challenge.

## EDP
Currently, we are in the first part of the EDP (Engineering Design Process) which is defining the problem. The problem I am facing Is finding an airplane calculator that is for a propeller airplane and that is free. Most people in the flightsim world like to give things for free and some like to be paid.


[Next](entry02.md)

[Home](../README.md)