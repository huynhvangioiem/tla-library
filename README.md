# TLA Library

A small CSS/SCSS component library built in 2021 as a university project.

> **Outdated.** This is an early piece of work, kept for reference and no longer maintained.
> The home page (`index.html`) is the student CV page I made at the time, not a current profile.
> For up-to-date work, see my GitHub profile.
> The code dates from August–October 2021; commits from 2026 only update this README and the repository name.

## Overview

The repository holds two things:
- **UI Component Library** (`TLALib/`): a custom CSS framework with a grid system, buttons, navigation and toast notifications
- **Demo pages**: `index.html` is the old student CV page built with the library; `library.html` documents the components

## Live Demo

[TLA Library on GitHub Pages](https://huynhvangioiem.github.io/tla-library/) opens the old student CV page.
The component documentation is at [library.html](https://huynhvangioiem.github.io/tla-library/library.html).

## Features

- **12-Column Grid System**: Responsive layout with desktop, tablet (`col-m`) and mobile (`col-s`) columns
- **Buttons**: Multiple variants (primary, secondary, success, danger, warning, info, outline, rounded, social)
- **Navigation**: Dropdown menus with smooth transitions
- **Toast Notifications**: Animated notifications with auto-dismiss functionality
- **Form Elements**: a single `.form-control` rule that makes an input full width

## Technologies

- HTML5
- CSS3 / SCSS
- JavaScript / jQuery
- Font Awesome 5.15.4
- Highlight.js (for code examples)

## Project Structure

```
tla-library/
├── TLALib/                    # Component library source
│   ├── CSS/
│   │   └── TLA.css           # Compiled library CSS
│   ├── JS/
│   │   └── TLA.js            # Library JavaScript
│   └── SCSS/                  # SCSS source files
│       ├── TLA.scss          # Main entry point
│       ├── _config.scss      # Colors & spacing config
│       ├── _layout.scss      # Grid system
│       ├── _nav.scss         # Navigation styles
│       ├── _button.scss      # Button components
│       ├── _toast.scss       # Toast notifications
│       ├── _form.scss        # Form styles
│       └── _reset.scss       # CSS reset
├── img/                       # Image assets
├── index.html                 # Old student CV page
├── library.html               # Library documentation
├── script.js                  # Main JavaScript
├── style.css                  # Main stylesheet
├── TLALibrary.vs1.min.css    # Minified library CSS
└── TLALibrary.vs1.min.js     # Minified library JS
```

## Usage

### Grid System

```html
<div class="row">
  <div class="col-6 col-m-12 col-s-12">Column 1</div>
  <div class="col-6 col-m-12 col-s-12">Column 2</div>
</div>
```

### Buttons

```html
<button class="btn btn-primary">Primary</button>
<button class="btn btn-outline-success">Outline Success</button>
<button class="btn btn-rounded btn-danger">Rounded Danger</button>
```

### Toast Notifications

```javascript
toast({
  title: "Success",
  message: "Your action was completed successfully!",
  style: "success",
  duration: 5000
});
```

## Color Palette

| Color     | Hex Code  |
|-----------|-----------|
| Primary   | `#0069d9` |
| Secondary | `#5a6268` |
| Success   | `#218838` |
| Danger    | `#c82333` |
| Warning   | `#e0a800` |
| Info      | `#138496` |
| Light     | `#e2e6ea` |
| Dark      | `#23272b` |

## Responsive Breakpoints

- **Desktop**: default styles
- **Tablet** (`col-m`): 1024px and below
- **Mobile** (`col-s`): 740px and below

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/huynhvangioiem/tla-library.git
   ```

2. Open `index.html` in your browser to view the old CV page

3. Open `library.html` to view the component library documentation

### Using the Library in Your Project

Include the minified CSS and JS files:

```html
<link rel="stylesheet" href="TLALibrary.vs1.min.css">
<script src="TLALibrary.vs1.min.js"></script>
```

Or include the full versions for development:

```html
<link rel="stylesheet" href="TLALib/CSS/TLA.css">
<script src="TLALib/JS/TLA.js"></script>
```

## Author

**Huynh Van Gioi Em (TLA)**

- Email: huynhvangioiem@gmail.com
- GitHub: [@huynhvangioiem](https://github.com/huynhvangioiem)

## License

This project is open source and available for personal and educational use.

---

© 2021 TLA. All rights reserved.
