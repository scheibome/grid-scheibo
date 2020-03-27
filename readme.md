# Grid-Scheibo - A Simple SCSS Grid Based on Flexbox

[![npm version](https://badge.fury.io/js/grid-scheibo.svg?style=flat)](https://npmjs.org/package/grid-scheibo)
 [![Issues](https://img.shields.io/github/issues/scheibome/grid-scheibo.svg)]( https://github.com/scheibome/grid-scheibo/issues) ![npm](https://img.shields.io/npm/dt/grid-scheibo.svg)
![npm](https://img.shields.io/npm/l/grid-scheibo.svg)

Demo (https://scheibome.github.io/grid-scheibo/)

## Install

``npm install grid-scheibo``

---

## Usage

#### Grid with CSS Grid
```
@import
'../../../node_modules/grid-scheibo/source/variables',
'../../../node_modules/grid-scheibo/source/cssgrid-scheibo';
```

#### Grid with Flexbox
```
@import
'../../../node_modules/grid-scheibo/source/variables',
'../../../node_modules/grid-scheibo/source/grid-scheibo';
```

---

## Advanced Usage

Insert your settings before the import

```
// add own gutter size
$col-gutter-size: 2rem;

// your grid with CSS-Grid
$grid-setup: (
  '1-1': '1fr 1fr',
  '1-1-1': '1fr 1fr 1fr',
  '1-2-1': '1fr 2fr'
);

// your grid with flexbox
$col-widths: (
  '1\\/8': '1/8',
  '2\\/8': '2/8',
  '3\\/8': '3/8',
  '4\\/8': '4/8',
  '5\\/8': '5/8',
  '6\\/8': '6/8',
  '7\\/8': '7/8',
  'full': 100%
);

// your breaks
$col-grid-breaks: (
  tablet: '900px',
  desktop: '1024px',
  wide: '1400px'
);

// for using CSS-Grid
@import '../../../node_modules/grid-scheibo/source/cssgrid-scheibo';
// for using Flexbox
@import '../../../node_modules/grid-scheibo/source/grid-scheibo';
```

### Examples

#### Grid with CSS-Grid

```
<div class="o-grid o-grid-1-1 o-grid-1-1-1@tablet o-grid-1-2-1@desktop">
  <div>Your Content</div>
  <div>Your Content</div>
  <div>Your Content</div>
  <div>Your Content</div>
  <div>Your Content</div>
  <div>Your Content</div>
  <div>Your Content</div>
  <div>Your Content</div>
</div>
```


#### Grid with Flexbox

#####  o-row--nogutter

```
<div class="o-row o-row--nogutter">
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-full@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-full@tablet o-row__col-1/4@desktop">Your Content</div>
</div>
```


##### o-row--between

```
<div class="o-row o-row--between">
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-full@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-full@tablet o-row__col-1/4@desktop">Your Content</div>
</div>
```

##### o-row--between & o-row--vertical-align

```
<!-- o-row--between & o-row--vertical-align -->
<div class="o-row o-row--between o-row--vertical-align">
  <div class="o-row__col-full o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-full o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-full@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
  <div class="o-row__col-1/2 o-row__col-1/3@tablet o-row__col-1/2@desktop">Your Content</div>
  <div class="o-row__col-full o-row__col-1/3@tablet o-row__col-1/4@desktop">Your Content</div>
</div>
```

##### o-row--row-reverse

```
<div class="o-row o-row--between o-row--vertical-align o-row--row-reverse@desktop">
  <div class="o-row__col-full o-row__col-1/3@tablet">Column 1</div>
  <div class="o-row__col-full o-row__col-1/3@tablet">Column 2</div>
  <div class="o-row__col-1/2 o-row__col-1/3@tablet">Column 3</div>
  <div class="o-row__col-1/2 o-row__col-full@tablet">Column 4</div>
</div>
```
