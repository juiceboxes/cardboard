# cardboard
Cardboard is not a UI library or framework, it's a starter kit to help you get off the ground in development.

## Installing
`npm install @juiceboxes/cardboard`

### Imports
Regular CSS: `@import 'node_modules/@juiceboxes/cardboard/cardboard.css'`

Minified CSS: `@import 'node_modules/@juiceboxes/cardboard/cardboard.min.css'`

SCSS with Variable declarations: `@import 'node_modules/@juiceboxes/cardboard/cardboard.scss'`

## Usage

###Components

Components are wrapped on the top level with a `jb-...` tag and then follows normal HTML structure.

#### Buttons

Variables:

`$jb-primary` and `jb-$accent`: Colors

Usage:

* Primary: `<button class='jb-button'> Button Text </button>` or `<button class='jb-button__primary'> Button Text </button>`

* Accent: ``<button class='jb-button__accent'> Button Text </button>``

#### Tables
Usage:
```html
<table class='jb-table'>
    <thead>
        <tr>
            <th> Table Header 1 </th>
            <th> Table Header 2 </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td> Table Data 1 </th>
            <td> Table Data 2 </th>
        </tr>
    <tbody>
</table>
```

### Layouts
Cardboard relies on [juice-grid](https://github.com/juiceboxes/juice-grid) for the grid layout and is included with the npm install if npm config is in development mode

#### Grid

Variables:

`$jb-grid-gutter`: spacing between grid elements, defaulted to `15px`.

Usage:

Basic
``` html
<div class="jb-grid">
    <div class="jb-row">
        <div class="jb-col-4">4 Columns</div>
        <div class="jb-col-8">8 Columns</div>
    </div>
</div>
```

With Gutters
``` html
<div class="jb-grid with-gutters">
    .
    .
    .
</div>
```

Offsetting Columns
``` html
<div class="jb-grid">
    <div class="jb-row">
        <div class="jb-col-4 jb-push-8">4 Column span starting at column 9 (spans col 9, 10 ,11 ,12)</div>
    </div>
</div>
```

#### Container
Should wrap page

Variables:

`$jb-container-width`: Width of your page. Defaulted to `80%`.

Usage: 
```html
<div class='jb-container'>
    .
    .
    .
</div>
```
