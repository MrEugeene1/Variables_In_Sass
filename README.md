# Variables in Sass

A concise Sass starter focused on using variables to improve consistency, readability, and maintainability in stylesheets.

## Overview

This project demonstrates a foundational Sass workflow by defining reusable design values (for example, text color) and applying them across the stylesheet.

Current implementation includes:
- A global `$font-color` variable
- Base `body` styling using the variable
- Clean default page spacing and background setup

## Tech Stack

- Sass (`.scss`)
- CSS (compiled output)

## Project Structure

```text
Variables_Sass/
├── styles.scss
└── README.md
```

## Sass Example in This Project

```scss
$font-color: #333;

body {
  color: $font-color;
}
```

## Getting Started

### 1. Install Sass

If Sass is not installed globally:

```bash
npm install -g sass
```

### 2. Compile SCSS to CSS

Run a one-time build:

```bash
sass styles.scss styles.css
```

Or run in watch mode during development:

```bash
sass --watch styles.scss:styles.css
```

## Why Use Variables?

Sass variables help you:
- Centralize design values
- Reduce repeated hard-coded values
- Update styles faster and with fewer mistakes
- Keep styling decisions consistent across files

## Recommended Next Improvements

To scale this starter into a production-ready styling foundation, consider:
- Creating additional variables for spacing, typography, and breakpoints
- Splitting styles into partials (for example, `_variables.scss`, `_base.scss`)
- Introducing maps or mixins for repeated patterns
- Adding linting/formatting for consistent style quality

## Example Variable Expansion

```scss
$font-color: #333;
$bg-color: #f4f4f4;
$font-family-base: Arial, sans-serif;

body {
  font-family: $font-family-base;
  color: $font-color;
  background-color: $bg-color;
  margin: 0;
  padding: 0;
}
```

## License

For learning and educational use.

