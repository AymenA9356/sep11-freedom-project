# Entry 3
##### 2/5/2024

## Intro/Context


Between the blog 2 and bolg 3 I have learned alot of things that will help me get closer and closer to my goal of makeing a plane calculator. The things i have learned so far are `.add()` `.addBack()``.after()` , `.addClass()`. These are going to be important for my learning as these give me a basic understanding of jQuery. As these basic understandings of jquery Increase I can then start to do more challenging things, but for now we are starting with the small step.


## Learning jQuery

In my time in learning my tool I have tried to be profisent in my understanding. So what I did was write what that code spacificly did and also add some explanations too. For the first code that I have tried to learn was `.add()`. So what does `.add()` even do? and what is its purrpose? `.add()` Create a new jQuery object with elements added to the set of matched elements. For Example:
```js
$(document).ready(function(){
    // Selecting all list items
    var listItems = $("li");

    // Adding a class to the selected list items
    listItems = listItems.add(".additional-list-item");
    });
```
In this example, the `.add()` function is used to add the list item with the class `.additional-list-item` to the set of list items selected by `$("li")`.

Another function I have leanred was the `.after()`.`.after()` function Inserts content, specified by the parameter, after each element in the set of matched elements.
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
 So we can see that after we used the .after() a new parigraph is made with the string "Test" in it.
 so first we see a class called `inner` and then we tell jquery to add a `<p></p>` after every class that have that and we get this
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











[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)