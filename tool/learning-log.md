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
<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->

