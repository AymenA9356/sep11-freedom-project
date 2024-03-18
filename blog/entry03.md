# Entry 3
##### 2/5/2024

## Intro/Context


Between blog 2 and blog 3, I have learned a lot of things that will help me get closer and closer to my goal of making a plane calculator. The things I have learned so far are `.add()` `.addBack()``.after()` , `.addClass()`. These are going to be important for my learning as these give me a basic understanding of jQuery [documentation](https://api.jquery.com/). As these basic understandings of jQuery Increase, I can then start to do more challenging things, but for now, we are starting with the small step.


## Learning jQuery

In my time learning my tool, I have tried to be proficient in my understanding. So what I did was write what that code specifically did and also add some explanations. The first code that I tried to learn was `.add()`. So what does `.add()` even do? and what is its purpose? `.add()` Create a new jQuery object with elements added to the set of matched elements. For Example:
```js
$(document).ready(function(){
    // Selecting all list items
    var listItems = $("li");

    // Adding a class to the selected list of items
    listItems = listItems.add(".additional-list-item");
    });
```
In this example, the `.add()` function is used to add the list item with the class `.additional-list-item` to the set of list items selected by `$("li")`.

Another function I have learned was the `.after()`.`.after()` function Inserts content, specified by the parameter, after each element in the set of matched elements.
Example:
```html

<div class="container">
  <h2>Greetings</h2>
  <div class="inner">Hello</div>
  <div class="inner">Goodbye</div>
</div>
```
```js
$( ".inner" ).after( "<p>Test</p>" );
```
 So we can see that after we used the .after() a new paragraph is made with the string "Test" in it.
 so first we see a class called `inner` and then we tell jQuery to add a `<p></p>` after every class that has that and we get this
 result.
 RESULT:
 ```html
 <div class="container">
  <h2>Greetings</h2>
  <div class="inner">Hello</div>
  <p>Test</p>
  <div class="inner">Goodbye</div>
  <p>Test</p>
</div>
```
`.addBack()` Add the previous set of elements on the stack to the current set, optionally filtered by a selector.
Example:
```js
$(document).ready(function(){
    // Selecting all paragraphs and their parent divs
    var paragraphs = $("p").css("color", "blue");
    var divs = paragraphs.parent().css("border", "1px solid black");

    // Adding back the paragraphs to the selection
    divs.addBack().css("background-color", "lightgray");
});
```
```html
<div>
    <p>Paragraph 1</p>
</div>
<div>
    <p>Paragraph 2</p>
</div>
```
All paragraphs `(<p>)` are selected and styled with blue color.
Then, their parent `<div>` elements are selected and styled with a black border.
Finally, .addBack() is used to include the paragraphs back into the selection, and they are styled with a light gray background color.


The `.addClass()` function in jQuery is used to add one or more CSS classes to the selected elements. Here's an example:

```js
$(document).ready(function(){
    // Selecting an element by its ID and adding a CSS class to it
    $("#myElement").addClass("highlight");

    // Selecting multiple elements by their class and adding a CSS class to all of them
    $(".paragraphs").addClass("italic bold");
});
```
```html
<div id="myElement">This element will be highlighted.</div>

<!-- Multiple paragraphs with class "paragraphs" -->
<p class="paragraphs">Paragraph 1</p>
<p class="paragraphs">Paragraph 2</p>
```
The element with the ID "myElement" is selected using `$("#myElement")`, and the class "highlight" is added to it using `.addClass("highlight")`. Multiple paragraphs with the class "paragraphs" are selected using `$(".paragraphs")`, and the classes "italic" and "bold" are added to all of them using `.addClass("italic bold")`.


## Skills
During this process, I developed the ability **how to Learn**. I learned a great deal about Javascript that I never would have thought to know. This is helping me get closer to creating my Airplane calculator. Another skill I learned was **How to read** being able to read and also understand the documentation so I can learn the most.


## EDP
Currently, we are still in the second third of the Engineering Design Process (EDP), which includes doing a problem investigation. We may now seek solutions to the problem that we have identified and characterized. Many planes in the field of flight simulation simply provide you with the actual take-off speeds. But whether the runway is cold, dry, or wet is unknown to the plane's computer. As a result, I'm developing a calculator that will account for all of those variables, including air pressure, temperature, runway condition, wind speed, and direction.



[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)