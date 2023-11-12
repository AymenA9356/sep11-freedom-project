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

X/X/X:
* Text


<!--
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->

