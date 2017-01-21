`md-virtual-repeater` is a directive from [angular/material](https://github.com/angular/material).

## Demo

https://pioug.github.io/md-virtual-repeater/

Source: https://github.com/pioug/md-virtual-repeater/blob/gh-pages/index.html

## Why?

- Best implementation of the infinite list for Angular 1.x
- Standalone version (no dependency to Angular Material)
- Simple installation (no external CSS, no bundle tool required)
- Safe for minification ([DI annotation](https://docs.angularjs.org/guide/di) included)

## Installation

```bash
npm install @pioug/md-virtual-repeater
```

Include the script `virtual-repeater.js` in your HTML:

```html
<script src="node_modules/@pioug/md-virtual-repeater/virtual-repeater.js"></script>
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

```css
md-virtual-repeat-container {
  height: 100%;
  overflow-x: hidden;
  overflow-y: scroll;
  position: absolute;
  width: 100%;
}

md-virtual-repeat-container:-webkit-scrollbar {
  width: 0 !important;
}
```

## Documentation

- `mdVirtualRepeat`: https://material.angularjs.org/latest/api/directive/mdVirtualRepeat
- `mdVirtualRepeatContainer`: https://material.angularjs.org/latest/api/directive/mdVirtualRepeatContainer
