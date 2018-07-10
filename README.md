![Grid Size](https://img.shields.io/github/size/juiceboxes/cardboard/dist/cardboard.min.css.svg)
![Travis](https://img.shields.io/travis/juiceboxes/cardboard.svg)

# juiceboxes/cardboard

Cardboard is not a UI library or framework, it's a starter kit to help you get off the ground in development.

Relies on [juice-grid](https://github.com/juiceboxes/juice-grid) for CSS Grid and Flexbox Grid solutions

## Installing

`npm install @juiceboxes/cardboard`

### Imports

Regular CSS: `@import 'node_modules/@juiceboxes/cardboard/cardboard.css'`

Minified CSS: `@import 'node_modules/@juiceboxes/cardboard/cardboard.min.css'`

SCSS with Variable declarations: `@import 'node_modules/@juiceboxes/cardboard/cardboard.scss'`

[Normalize](https://github.com/necolas/normalize.css/): `@import 'node_modules/@juiceboxes/cardboard/normalize.css'`

## Usage

### Components

Components are wrapped on the top level with one element tag and then follows normal HTML structure.

#### Buttons

Variables:
Colors, lighter and darker colors are based on initial color

`$accent`: default: `#33C3F0`

Usage:

* Primary:

```html
<button class='button'> Button Text </button>
<a class='button'> Anchor Button Text </button>
<input class='button' type="submit" value="submit input"> Input Text </input>
<input class='button' type="button" value="submit input"> Input Text </input
```

* Accent:

```html
<button class='button accent'> Accent Button Text </button>
<a class='button accent'> Anchor Accent Button Text </button>
<input class='button accent' type="submit" value="submit input"> Accent Submit Input Text </input>
<input class='button accent' type="button" value="submit input"> Accent Button Input Tex </input>
```

#### Cards

Variables:

`$card__border-radius`: card border radius, default: `1.5px`

`$card__padding`: padding for card contents, default: `15px`

Usage:

* Primary:

```html
<button class='button'> Button Text </button>
<a class='button'> Anchor Button Text </button>
<input class='button' type="submit" value="submit input"> Input Text </input>
<input class='button' type="button" value="submit input"> Input Text </input
```

* Accent:

```html
<button class='button accent'> Accent Button Text </button>
<a class='button accent'> Anchor Accent Button Text </button>
<input class='button accent' type="submit" value="submit input"> Accent Submit Input Text </input>
<input class='button accent' type="button" value="submit input"> Accent Button Input Tex </input>
```

#### Tables

Variables:

`$table__border-color`: border color under the thead, default: `#c7c7c7`

`$table__background`: even row background color, default: `#c7c7c7`

Usage:

```html
<table class='table'>
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

#### Code

Usage:

```html
<pre><code>.foo {
    background: blue;
} </code></pre>
```

#### Headers/Titles

Variables:

`$header__font-size--max`: max size for headers, default: `4.0rem`;

Usage:

```html
<h1 class='title'> h1 Title </h1>
<h2 class='title'> h2 Title </h2>
.
.
.
```

#### Lists

Usage:

```html
<li class='list'>
    <li> List Item </li>
    <li> List Item </li>
    <ol class='list'>
        <li> Nested List Item </li>
        <li> Nested List Item </li>
    </ol>
</li>
```

### Layouts

Cardboard relies on [juice-grid](https://github.com/juiceboxes/juice-grid) for the grid layout and is included with the npm install -- if npm config is in development mode

#### Container

Should wrap page

Variables:

`$container__width`: Width of your page, Default: `80%`.

Usage:

```html
<div class='container'>
    .
    .
    .
</div>
```
