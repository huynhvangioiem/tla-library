# TLA Library

A small CSS/SCSS component library I wrote at university: a 12-column grid, buttons, a dropdown navigation bar and animated toast messages. It is built with SCSS and jQuery, and it is dated now. I keep it as an early piece of work.

**Live demo:** [huynhvangioiem.github.io/tla-library](https://huynhvangioiem.github.io/tla-library/) — the documentation page, with a live example and code for each component.

## What is in it

- **Grid**: 12 columns with `col-N`, `col-m-N` (tablet) and `col-s-N` (mobile) classes, plus offsets such as `col-o-1`.
- **Buttons**: `btn` with a colour (`btn-primary`, `btn-secondary`, `btn-success`, `btn-danger`, `btn-warning`, `btn-info`, `btn-light`, `btn-dark`), `btn-outline-*`, `btn-rounded` and `btn-social`.
- **Navigation**: `navbar` with nested dropdowns and a toggle button on small screens.
- **Toast**: `toast({ title, message, style, duration, iconType })` shows an animated message that closes itself.
- **Forms**: only `.form-control { width: 100% }` for now.

## Use it

Include the library after jQuery and Font Awesome (the toast and navbar icons use Font Awesome):

```html
<link rel="stylesheet" href="TLALib/CSS/TLA.css">
<script src="TLALib/JS/TLA.js"></script>
```

Minified copies are in `TLALibrary.vs1.min.css` and `TLALibrary.vs1.min.js`.

### Grid

```html
<div class="row">
  <div class="col-6 col-m-12 col-s-12">Column 1</div>
  <div class="col-6 col-m-12 col-s-12">Column 2</div>
</div>
```

### Buttons

```html
<button class="btn btn-primary">Primary</button>
<button class="btn btn-outline-success">Outline success</button>
<button class="btn btn-rounded btn-danger">Rounded danger</button>
```

### Toast

Add an empty `<div id="toast"></div>` to the page, then:

```javascript
toast({
  title: "Success",
  message: "Your action was completed.",
  style: "success", // or "success-colored", "success-outline", ...
  duration: 5000,
});
```

## Breakpoints

| Range | Used for |
|-------|----------|
| 1441px and up | large desktop |
| 1025px – 1280px | desktop |
| 741px – 1024px | tablet (`col-m-*`) |
| 740px and below | mobile (`col-s-*`) |

## Structure

```
index.html          documentation page
style.css           styles for the documentation page (compiled from SCSS/)
script.js           helpers for the documentation page
SCSS/               source of style.css
TLALib/             the library: CSS/, JS/ and SCSS/ source
TLALibrary.vs1.min.*  minified build
```

## Author

Huynh Van Gioi Em — [@huynhvangioiem](https://github.com/huynhvangioiem)
