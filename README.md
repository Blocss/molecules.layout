# Blocss Layout – v0.0.0

A [Blocss](https://github.com/Blocss/blocss/) component for a CSS layout system. Layout makes use of `flexbox` and
`box-sizing` to provide features that float-based layouts cannot.

**N.B.** This component relies on particular dimensions being applied to cells in
the grid via other classes. For example the [Blocss dimensions](https://github.com/Blocss/dimensions/) extension.

Read more about [Blocss](https://blocss.github.io/blocss).

## Installation

    $ bower install --save blocss-layout

## Features

* Fluid layout.
* Intelligent cell wrapping.
* Horizontal centering of cells.
* Custom vertical alignment of cells (top, bottom, or middle).
* Cell width is controlled independently of grid gutter.
* Infinite nesting.
* Built-in redundancy.

## Available classes

* `.layout`: core component

## Available settings

* `$blocss-layout-namespace` - Prefixes classes with a namespace, defaults to `$blocss-namespace`

## Use

A simple layout is easy to create. A layout container can have any number of child
cells.

```html
```

## Deprecated
All the api calls which are deprecated: none

## Browser support

* Google Chrome (latest)
* Opera (latest)
* Firefox 4+
* Safari 5+
* Internet Explorer 10+
