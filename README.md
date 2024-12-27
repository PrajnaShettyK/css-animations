# css-animations

Let’s delve into the code step by step to understand and master CSS animations.

### HTML Structure

The HTML structure begins with the DOCTYPE declaration, specifying the document type as HTML5.

```html
<!DOCTYPE html>
```

Next, we have the HTML tags, which are the root element that encloses the entire document.

```html
<html lang=“en”>
```

The head section contains metadata and links for external resources, including the CSS file.

```html
<head>
  <meta charset=“UTF-8”>
  <meta name=“viewport” content=“width=device-width, initial-scale=1.0”>
  <title>Classy cards</title>
  <link rel=“stylesheet” href=“style.css”>
</head>
```

The meta tags define the character set (UTF-8) and make the page responsive by adjusting it to the user’s device width.

The link tag links an external CSS file (style.css) for styling.

The body section contains all the visible elements, such as the cards.

### Card Layout in HTML

Each card follows a specific structure:

```html
<div class=“card color-class”>
  <div class=“card-header”>…</div>
  <div class=“card-body”>…</div>
  <div class=“card-footer”>…</div>
</div>
```

Let’s break down each element:

- **card Class:** Defines the layout and styling of the card.
- **card-header:** Displays a date and an SVG icon.

```html
<div class=“card-header”>
  <div class=“date”>Feb 2, 2021</div>
  <svg>…</svg>
</div>
```

- **card-body:** Contains the main content, such as the title, description, and progress bar.

```html
<div class=“card-body”>
  <h3>web designing</h3>
  <p>Prototyping</p>
  <div class=“progress”>
    <span>Progress</span>
    <div class=“progress-bar”></div>
    <span>90%</span>
  </div>
</div>
```

- **card-footer:** Contains avatars, a button for adding members, and a countdown.

```html
<div class=“card-footer”>
  <ul>
    <li><img src=“image_url” alt=“”></li>
  </ul>
  <a href=“#” class=“btn-countdown”>2 days left</a>
</div>
