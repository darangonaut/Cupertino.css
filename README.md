# Cupertino.css

**Apple-inspired Classless CSS Framework**

Cupertino.css is a lightweight, classless CSS framework inspired by Apple’s design language. It provides beautiful, modern, and responsive default styles for HTML elements, allowing you to create elegant web pages with minimal effort and no custom classes.

## Features

- 🍏 **Apple-inspired Design:** Clean, modern aesthetic with SF Pro-like typography.
- 🎨 **Classless:** Styles default HTML tags directly.
- 🌫️ **Glassmorphism:** Native support for frosted glass effects (backdrop blur + saturation) in navigation and modals.
- 🌙 **Dark Mode:** Automatic support based on system preferences (`color-scheme` aware native controls).
- 🎚️ **iOS Controls:** Custom styles for Switches, Sliders, Selects, Checkboxes, and Radios.
- 🧩 **Rich Defaults:** Styled tables, messages/alerts, accordions, cards, badges, blockquotes, code blocks, and pagination.
- ♿ **Accessible:** Visible `:focus-visible` rings on all interactive elements; respects `prefers-reduced-motion`.
- 📱 **Responsive:** Mobile-first approach with balanced typography.

## Installation

### 1. Using CDN (Recommended)
The easiest way to use Cupertino.css is to include it via jsDelivr CDN. Just add this line to your `<head>`:

```html
<!-- Always get the latest version (not recommended for production) -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/darangonaut/Cupertino.css/cupertino.css">

<!-- Or use a specific version (recommended) -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/darangonaut/Cupertino.css@v1.0.1/cupertino.css">
```

### 2. Manual Installation
Download the `cupertino.css` file and include it in your project:

```html
<link rel="stylesheet" href="cupertino.css" />
```

## Usage & Components

Just add the stylesheet to your HTML file. Most elements work automatically, but here are some specific iOS-style components:

### 1. Toggle Switch
To create an iOS-style toggle switch, simply add `role="switch"` to a checkbox:

```html
<label>
  <input type="checkbox" role="switch" checked>
  Wi-Fi
</label>
```

### 2. Glassmorphism Dialog
Use the native `<dialog>` element. It automatically gets the frosted glass backdrop and rounded corners.

```html
<dialog id="my-dialog">
  <h3>System Alert</h3>
  <p>This dialog features a glassmorphism backdrop.</p>
  <form method="dialog">
    <button>Close</button>
  </form>
</dialog>

<button onclick="document.getElementById('my-dialog').showModal()">Open Dialog</button>
```

### 3. Navigation Bar
 The `<nav>` element automatically applies a sticky, semi-transparent frosted glass effect to the top of the page.

```html
<nav>
  <ul>
    <li><a href="#home">Home</a></li>
    <li><a href="#about">About</a></li>
  </ul>
</nav>
```

### 4. Messages & Alerts
Use the `<aside>` element. The `role` attribute switches the accent color (default → blue/gray, `status` → green, `alert` → red).

```html
<aside><strong>Info:</strong> A general message.</aside>
<aside role="status"><strong>Success:</strong> Saved!</aside>
<aside role="alert"><strong>Error:</strong> Something went wrong.</aside>
```

### 5. Range Slider
A plain range input gets an iOS-style track and thumb automatically.

```html
<input type="range" min="0" max="100" value="50">
```

### 6. Loading Button
Add the `loading` class to a button to show a spinner and disable interaction.

```html
<button class="loading">Saving…</button>
```

Other styled elements work out of the box with semantic markup: `<table>`, `<blockquote>`, `<details>`/`<summary>` (accordion), `<mark>` (badge), `<kbd>`, `<progress>`, and a `.pagination` container.

## Standard HTML Example

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>My Cupertino.css Page</title>
    <link rel="stylesheet" href="cupertino.css" />
  </head>
  <body>
    <nav>...</nav>
    <main>
      <h1>Hello, Cupertino.css!</h1>
      <p>This page uses Apple-inspired classless styles.</p>
      <button>Button</button>
      <button class="secondary">Secondary</button>
    </main>
  </body>
</html>
```

## Browser Support

Cupertino.css ships as a single file with no build step and uses modern CSS — native nesting (`&`), `:has()`, `color-mix()`, and `@supports`. It targets evergreen browsers (Chrome/Edge 120+, Safari 17+, Firefox 121+). On older engines styling degrades gracefully to readable defaults.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request on GitHub.

## License

This project is licensed under the MIT License.