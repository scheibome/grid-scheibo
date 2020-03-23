# Grid-Scheibo - a simple scss grid based on flexbox

[![npm version](https://badge.fury.io/js/grid-scheibo.svg?style=flat)](https://npmjs.org/package/grid-scheibo)
 [![Issues](https://img.shields.io/github/issues/scheibome/grid-scheibo.svg)]( https://github.com/scheibome/grid-scheibo/issues) ![npm](https://img.shields.io/npm/dt/grid-scheibo.svg)
![npm](https://img.shields.io/npm/l/grid-scheibo.svg)


## Install

``npm install grid-scheibo``

---

## Usage

```
@import
'../../../node_modules/grid-scheibo/source/variables',
'../../../node_modules/grid-scheibo/source/grid-scheibo';
```

---

## Advanced usage

Insert your settings before the import

```
// add own gutter size
$col-gutter-size: 2rem;

// your grid
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

@import '../../../node_modules/grid-scheibo/source/grid-scheibo';
```
