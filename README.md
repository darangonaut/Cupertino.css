# Cupertino.css

**Apple-inspired Classless CSS Framework**

Cupertino.css is a lightweight, classless CSS framework inspired by Apple’s design language. It provides beautiful, modern, and responsive default styles for HTML elements, allowing you to create elegant web pages with minimal effort and no custom classes.

## Features

- 🍏 **Apple-inspired Design:** Clean, modern aesthetic with SF Pro-like typography.
- 🎨 **Classless:** Styles default HTML tags directly.
- 🌫️ **Glassmorphism:** Native support for frosted glass effects (backdrop blur + saturation) in navigation and modals.
- 🌙 **Dark Mode:** Automatic support based on system preferences.
- 🎚️ **iOS Controls:** Custom styles for Switches, Sliders, and Selects.
- 📱 **Responsive:** Mobile-first approach with balanced typography.

## Installation

### 1. Using CDN (Recommended)
The easiest way to use Cupertino.css is to include it via jsDelivr CDN. Just add this line to your `<head>`:

```html
<!-- Always get the latest version (not recommended for production) -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/darangonaut/Cupertino.css/cupertino.css">

<!-- Or use a specific version (recommended) -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/darangonaut/Cupertino.css@v1.0.0/cupertino.css">
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

## Contributing

Contributions are welcome! Please open an issue or submit a pull request on GitHub.

## License

This project is licensed under the MIT License.