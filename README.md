# Mere-css-utility

A set of basic CSS classes to facilitate the development process.

### Features

* Small size (3kb - minified);
* There are base styles for normalizing a document;
* Only the necessary minimum of CSS classes;
* Unified custom indents.

---

## Getting Started


### Installation

```console
npm i mere-css-utility
```

### Quick Start 

In your scss file:

```
@import "node_modules/mere-css-utility/scr/mere";

------------------------------------
or you can use only needed packages
------------------------------------

@import 'node_modules/mere-css-utility/scr/utility/base';
@import 'node_modules/mere-css-utility/scr/utility/displays';
@import 'node_modules/mere-css-utility/scr/utility/flexbox';
@import 'node_modules/mere-css-utility/scr/utility/indents';
@import 'node_modules/mere-css-utility/scr/utility/typography';
```

---

## Documentation

### Displays

In your scss file: `@import "node_modules/mere-css-utility/scr/utility/displays"`

CSS class  | Meaning
------------- | -------------
.d-inline  | display: inline
.d-inline-block  | display: inline-block
.d-block  | display: block
.d-flex  | display: flex

### Flexbox

In your scss file: `@import "node_modules/mere-css-utility/scr/utility/flexbox"`

CSS class  | Meaning
------------- | -------------
.ai-flex-start  | align-items: flex-start
.ai-flex-end  | align-items: flex-end
.ai-center  | align-items: center
.jc-flex-start  | justify-content: flex-start
.jc-flex-end  | justify-content: flex-end
.jc-center  | justify-content: center
.jc-space-between  | justify-content: space-between
.jc-space-around  | justify-content: space-around
.fd-row  | flex-direction: row
.fd-row-reverse  | flex-direction: row-reverse
.fd-column  | flex-direction: column
.fd-column-reverse  | flex-direction: column-reverse

### Typography

In your scss file: `@import "node_modules/mere-css-utility/scr/utility/typography"`

CSS class  | Meaning
------------- | -------------
.fs-1  | font-size: 0.75rem; line-height: 0.75rem
.fs-2  | font-size: 1rem; line-height: 1rem
.fs-3  | font-size: 1.25rem; line-height: 1.25rem
.fs-4  | font-size: 1.5rem; line-height: 1.5rem
.fs-5  | font-size: 2rem; line-height: 2rem
.fs-6  | font-size: 2.5rem; line-height: 2.5rem
.fw-light  | font-weight: light
.fw-normal  | font-weight: normal
.fw-medium  | font-weight: medium
.fw-bold  | font-weight: bold
.ta-center  | text-align: center
.ta-right  | text-align: right
.ta-left  | text-align: left
.tt-uppercase  | text-transform: uppercase
.tt-lowercase  | text-transform: lowercase
.tt-capitalize  | text-transform: capitalize

### Indents

In your scss file: `@import "node_modules/mere-css-utility/scr/utility/indents"`  

A set of classes mb, mt, mr, ml, pt, pb, pr, pl with number postfix from 0 to 5.  

Default `$base-indent: 8px`. If you want to rewrite base indent change the variable `$base-indent`.  

`${i}` - is the number of indentation, which is a factor for `$base-indent`  

For example `.mb-3` is equal `margin-bottom: 24px` (8px * 3) and `.mr-0` is equal `margin-right: 0` (8px * 0)

CSS class  | Meaning
------------- | -------------
.mb-${i}  | margin-bottom: ${i} * $base-indent
.mt-${i}  | margin-top: ${i} * $base-indent
.mr-${i}  | margin-right: ${i} * $base-indent
.ml-${i}  | margin-left: ${i} * $base-indent
.pb-${i}  | padding-bottom: ${i} * $base-indent
.pt-${i}  | padding-top: ${i} * $base-indent
.pr-${i}  | padding-right: ${i} * $base-indent
.pl-${i}  | padding-left: ${i} * $base-indent

### Base

In your scss file: `@import "node_modules/mere-css-utility/scr/utility/base"`  

This file contains base CSS styles for reset default browsers styles.
