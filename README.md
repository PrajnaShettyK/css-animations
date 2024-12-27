# css-animations
Explaination of the code in detail so you can understand and master it step by step:

1. Structure of the HTML
	•	DOCTYPE Declaration:
Specifies the document type as HTML5.
<!DOCTYPE html>
	•	HTML Tags:
The root element that encloses the entire document.
<html lang="en">
	•	Head Section:
Contains metadata and links for external resources like the CSS file:

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Classy cards</title>
  <link rel="stylesheet" href="style.css">
</head>

	•	meta Tags: Define the character set (UTF-8) and make the page responsive by adjusting it to the user’s device width.
	•	link Tag: Links an external CSS file (style.css) for styling.

	•	Body Section:
Contains all the visible elements, such as the cards.

2. Card Layout in HTML

Each card follows this structure:

<div class="card color-class">
  <div class="card-header">...</div>
  <div class="card-body">...</div>
  <div class="card-footer">...</div>
</div>

Breakdown:
	•	card Class: Defines the layout and styling of the card.
	•	card-header:
	•	Displays a date and an SVG icon.
	•	Example:

<div class="card-header">
  <div class="date">Feb 2, 2021</div>
  <svg>...</svg>
</div>


	•	card-body:
	•	Contains the main content, such as the title, description, and progress bar.
	•	Example:

<div class="card-body">
  <h3>web designing</h3>
  <p>Prototyping</p>
  <div class="progress">
    <span>Progress</span>
    <div class="progress-bar"></div>
    <span>90%</span>
  </div>
</div>


	•	card-footer:
	•	Contains avatars, a button for adding members, and a countdown.
	•	Example:

<div class="card-footer">
  <ul>
    <li><img src="image_url" alt=""></li>
  </ul>
  <a href="#" class="btn-countdown">2 days left</a>
</div>

3. CSS Styling (style.css)

General Rules:
	•	Reset styles:
Removes default padding and margins for all elements:

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}


	•	Body Styling:
Makes the body a full-screen centered container with a dark background:

body {
  min-height: 100vh;
  background: #232228;
  font-family: "Nunito", sans-serif;
  display: grid;
  place-items: center;
}



Card Styling:
	•	Card Layout:
Adds a shadow, rounded corners, and centering for the cards:

.card {
  box-shadow: 1px 12px 25px rgba(0, 0, 0, 0.78);
  border-radius: 2.25rem;
  display: grid;
  place-items: center;
}


	•	Card Variants:
Adds unique colors for different cards (e.g., green, red, orange, blue):

.green {
  background: radial-gradient(...);
}


	•	Progress Bar:
Represents progress visually with a filled bar:

.progress-bar:after {
  background: #01c3a8;
  width: 90%; /* Adjust based on progress */
}



Responsive Design:

The meta tag in the head and the flexible CSS units ensure the layout works well on all screen sizes.

4. Key Features
	•	Dynamic Styling:
Each card has a unique style defined by classes like .green or .red.
	•	Progress Indicators:
The progress bar visually represents progress with customizable percentages.
	•	Responsive Design:
Cards are centered and adapt to different screen sizes.

Practice Task
	1.	Customize the Colors:
Try changing the gradient colors in .green, .blue, etc.
	2.	Modify the Progress:
Adjust the width of .progress-bar:after to show different progress levels.
	3.	Add New Cards:
Create new cards by duplicating the existing structure and modifying the content.
	4.	Experiment with Fonts:
Change the font-family in the body selector to see how it affects the design.

Let me know if you’d like help with any specific section!
