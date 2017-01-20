`md-virtual-repeater` is a directive from [angular/material](https://github.com/angular/material).

## Why?

- Best implementation of the infinite list for Angular 1.x
- Standalone version (no dependency to Angular Material)
- Simple installation (no external CSS, no bundle tool required)
- Safe for minification ([DI annotation](https://docs.angularjs.org/guide/di) included)

## Installation

Include the script `virtual-repeater.js` in your HTML:

```html
<script src="node_modules/md-virtual-repeater/virtual-repeater.js"></script>
```

Load the Angular module `virtualRepeat` in your JS:

```js
angular.module('myAngularApp', ['virtualRepeat']);
```

## Usage

```html
<md-virtual-repeat-container md-top-index="topIndex">
  <div md-virtual-repeat="i in items" md-item-size="20">Hello {{i}}!</div>
</md-virtual-repeat-container>
```

## Documentation

- `mdVirtualRepeat`: https://material.angularjs.org/latest/api/directive/mdVirtualRepeat
- `mdVirtualRepeatContainer`: https://material.angularjs.org/latest/api/directive/mdVirtualRepeatContainer
