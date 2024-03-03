# Tool Learning Log

Tool: **jQuery**

Project: **Plane V-Speed calculator**

---

10/23/2023:
* **jQuery**: is to make it much easier to use JavaScript on your website
* DOM manipulation: jQuery makes it easy to select, manipulate, and traverse HTML elements in the Document Object Model (DOM).

```html
<!DOCTYPE html>
<html>
<head>
  <title>Simple jQuery Example</title>
  <!-- Include jQuery library -->
  <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
</head>
<body>

<button id="toggleButton">Toggle Paragraph</button>
<p id="myParagraph">This is a paragraph. Click the button to hide/show me.</p>

<script>
  // jQuery code
  $(document).ready(function() {
    // Attach a click event handler to the button
    $("#toggleButton").click(function() {
      // Toggle the visibility of the paragraph
      $("#myParagraph").toggle();
    });
  });
</script>

</body>
</html>
```

11/24/2023:


```js
$(document).ready(function() {
    // When the document is ready

    // API endpoint for fetching user data
    var apiEndpoint = 'https://jsonplaceholder.typicode.com/users';

    // Make an AJAX request to the API
    $.ajax({
        url: apiEndpoint,
        method: 'GET',
        success: function(users) {
            // Handle the successful response

            // Iterate through the retrieved users
            users.forEach(function(user) {
                // Create a card for each user and append it to the #users div
                var userCard = '<div class="user-card">';
                userCard += '<h2>' + user.name + '</h2>';
                userCard += '<p><strong>Email:</strong> ' + user.email + '</p>';
                userCard += '<p><strong>Username:</strong> ' + user.username + '</p>';
                userCard += '</div>';

                $('#users').append(userCard);
            });
        },
        error: function() {
            // This thing handels errors
            $('#users').html('<p>Error fetching data from the API.</p>');
        }
    });
});
```
* $(document).ready(function() { ... }): This ensures that the jQuery code runs when the document is fully loaded.

* var apiEndpoint = 'https://jsonplaceholder.typicode.com/users';: Specifies the API endpoint to fetch user data.

* $.ajax({ ... }): Initiates an AJAX request to the specified API endpoint.
success: function(users) { ... }: Handles the successful response from the API.
Inside the success callback, a loop iterates through each user and dynamically creates a user card with HTML.

* $('#users').append(userCard);: Appends the user card to the #users div.
* error: function() { ... }: Handles errors in case the API request fails.



12/4/2023

learned on how to grabe the element of a list using Jquery.

**12/18/2023 BLOG 3**

`.add()`
* Create a new jQuery object with elements added to the set of matched elements


`.addBack()`
* Add the previous set of elements on the stack to the current set, optionally filtered by a selector.
for example
```html
<ul>
  <li>list item 1</li>
  <li>list item 2</li>
  <li class="third-item">list item 3</li>
  <li>list item 4</li>
  <li>list item 5</li>
</ul>
```
```javascript

$( "li.third-item" ).nextAll().addBack()
  .css( "background-color", "red" );
  ```
  So what does this do? So in the list we have a class that is called `third item`. we then add a `.nextAll` so Jquery added everything that is after that class and then we call the css file and make the background color red>


`.addClass()`
* Adds the specified class(es) to each element in the set of matched elements.


`.after()`
* Insert content, specified by the parameter, after each element in the set of matched elements.
Example
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
Week 3-3-2024
[.Empty and .remove Video](https://www.youtube.com/watch?v=nYBa0UGLn4g&list=PL4cUxeGkcC9hNUJ0j6ccnOAcJIPoTRpO4&index=11)

This video talk about how we can use `.empty` and `.remove`. `.empty` emptys content what ever is inside it, Eample:
`$(".button").empty()`
What ever was in the element button it would be gone but the element would not be dealeted.


Ther is also anotherone called `.remove`. This takes the element and snapes it out of existance like what Thanos did, Eample:
`$(".button").remove()`
This will dealete the element and what ever is inside it.





<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->



