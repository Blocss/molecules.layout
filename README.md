# Blocss Layout – v0.1.1

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

* `.layout`: Root module
* `.layout--align-center`: Center align cells
* `.layout--align-right`: Right align cells
* `.layout--align-middle`: Vertical align cells to middle
* `.layout--align-bottom`: Vertical align cells to bottom
* `.layout--fit`: Vertical Allow cells to equal distribute width
* `.layout--equalheight`: All cells match height of tallest cell in a row, requires direct child of `.layout__cell` to be a single element
* `.layout--gutter`: Adds a default gutter between all cells
* `.layout--gutter-tiny`: Adds a tiny gutter between all cells
* `.layout--gutter-small`: Adds a small gutter between all cells
* `.layout--gutter-large`: Adds a large gutter between all cells
* `.layout--gutter-huge`: Adds a huge gutter between all cells
* `.layout__cell`: Cell element, always needs to be direct child of `.layout`, defaults to be 100% wide.
* `.layout__cell--center`: Center aligns this cell
* `.layout__cell--fit`: Make a cell shrink wrap its content.
* `.layout__cell--fill`: Make a cell fill the remaining space.


## Available settings

* `$blocss-layout-namespace` - Prefixes classes with a namespace, defaults to `$blocss-namespace`
* `$blocss-dimensions-responsive-modifier` - Prefixes responsive classes, defaults to `$blocss-responsive-modifier`
* `$blocss-use-layout` - Enables/disables the entire module, defaults to `true`
* `$blocss-layout-gutter` - Defines the gutter width, defaults to `$blocss-space`
* `$blocss-layout-gutter-tiny` - Defines the tiny gutter width, defaults to `$blocss-space-tiny`
* `$blocss-layout-gutter-small` - Defines the small gutter width, defaults to `$blocss-space-small`
* `$blocss-layout-gutter-large` - Defines the large gutter width, defaults to `$blocss-space-large`
* `$blocss-layout-gutter-huge` - Defines the huge gutter width, defaults to `$blocss-space-huge`
* `$blocss-dimensions-breakpoint-has-fit` - Defines the breakpoints where `.layout__cell--fit` can be applied to, defaults to `()`.
* `$blocss-dimensions-breakpoint-has-fill` - Defines the breakpoints where `.layout__cell--fill` can be applied to, defaults to `()`.

## Use

A simple layout is easy to create. A layout container can have any number of child
cells.

```html
<div class="layout  [layout--align-center|layout--align-right|layout--align-middle|layout--align-bottom|layout--fit|layout--equalheight|layout--gutter]">
    <div class="layout__cell  [layout__cell--center|layout__cell--fit|layout__cell-fill]"></div>
    <div class="layout__cell  [layout__cell--center|layout__cell--fit|layout__cell-fill]"></div>
    <div class="layout__cell  [layout__cell--center|layout__cell--fit|layout__cell-fill]"></div>
    <div class="layout__cell  [layout__cell--center|layout__cell--fit|layout__cell-fill]"></div>
</div>
```

## Deprecated
All the api calls which are deprecated: none

## Browser support

* Google Chrome (latest)
* Opera (latest)
* Firefox 4+
* Safari 5+
* Internet Explorer 10+

*NOTE*: For some of the supported browsers you need to add browserprefixes, most likely this already happens in your build process
