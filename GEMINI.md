# Project: Cupertino.css

## Project Overview

Cupertino.css is a lightweight, classless CSS framework inspired by Apple’s design language. It provides beautiful, modern, and responsive default styles for HTML elements, allowing you to create elegant web pages with minimal effort and no custom classes. The project consists of a single CSS file, `cupertino.css`, and an `index.html` file that serves as a live demonstration of the framework's features.

**Key Technologies:**

*   **CSS:** The core of the project is a single CSS file with a comprehensive set of styles for all standard HTML elements.
*   **HTML:** The `index.html` file showcases the framework's capabilities.

**Architecture:**

The framework is "classless," meaning it styles default HTML tags directly, eliminating the need for custom CSS classes. It uses CSS variables for a consistent design system (colors, fonts, spacing) and includes a dark mode theme that automatically activates based on user preferences.

## Building and Running

There is no build process for this project. To use the framework, simply include the `cupertino.css` file in your HTML.

To view the example page, open the `index.html` file in a web browser. The `index.html` file has been updated with comments to highlight the newly styled elements.

```html
<link rel="stylesheet" href="cupertino.css" />
```

## Development Conventions

*   **Styling:** The CSS is well-structured and uses variables for easy customization. It follows a standard format with sections for reset, base styles, typography, forms, and components.
*   **Dark Mode:** The framework includes a dark mode that is automatically enabled based on the user's system preferences using the `prefers-color-scheme` media query.
*   **Responsiveness:** The framework is designed to be responsive and mobile-friendly, with a media query for smaller screens.
*   **No Build Tools:** The project is simple and does not require any build tools or package managers.

### Styled Elements

The following HTML elements and classes have been styled to enhance the Apple-inspired design:

*   **Messages & Alerts (`<aside>`):** Provides distinct visual styles for informational, success (`aside[role="status"]`), and error (`aside[role="alert"]`) messages.
*   **Accordion (`<details>`, `<summary>`):** Styled to create an interactive, collapsible content area with custom arrow indicators.
*   **Progress Bar (`<progress>`):** Given an Apple-like appearance with custom styling for the progress bar and its value.
*   **Keyboard Shortcuts (`<kbd>`):** Styled to visually represent keyboard keys, similar to Apple's documentation.
*   **Badges and Tags (`<mark>`):** Styled to function as small, highlighted badges or tags.
*   **Loading Button (`.loading` class):** Adds a visual loading spinner animation to buttons when the `.loading` class is applied.
*   **Unordered Lists (`<ul>`):** The styling for unordered lists has been adjusted to ensure custom bullet points are correctly positioned and do not overlap with the text.
