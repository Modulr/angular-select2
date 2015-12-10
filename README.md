# Angular Select2
Angular Select2 is an Angularjs component that can replacement for select boxes.

- [Demo](http://modulr.io/components/angular-select2/)

![](http://modulr.io/img/preview/angular-select2.png)

##Features

- Uses the native Angularjs scope for data binding
- Remote data support
- Big data support


##Requirements

- [Angularjs](https://angularjs.org/)
- [Bootstrap 3.](http://getbootstrap.com/)
- [Selec2.](https://select2.github.io/)

##Quick start

Several quick start options are available:

- [Download the latest release](https://github.com/Modulr/angular-select2/archive/master.zip)
- Clone the repo: `git clone https://github.com/Modulr/angular-select2.git`.
- Install with [Bower](http://bower.io/): `bower install angular-mdr-select2`.
- Install with [npm](https://www.npmjs.com): `npm install angular-mdr-select2`.

##What's included

```
angular-select2/
  dist/
    ├── angular-select2.js
    └── angular-select2.min.js
```

##Documentation

####Usage

######Load JS

```html
<script href="angular-select2/dist/angular-select2.min.js"></script>
```

######Code

```js
angular.module('MyApp', ['mdr.select2'])
```

######HTML View or Templates

> Basic Directive

```html
<mdr-select2 url="http://miserver.com/json" options="item.estate for item in collection track by item.id"></mdr-select2>
```

> Complete Directive (All attributes)

```html
<select2 src="collection" options="item.estate group by item.zone for item in collection | orderBy:'item' track by item.id" model="model" selected="value" placeholder="Seleccionar" disabled="true" required></select2>
```

####API

######Attributes

Attribute | Type | Description
--- | --- | ---
url | `string` | *Is the path where you get list of items.*
src | `array` | *Collection of objects*
options | `string` | *Dynamically generate a list of <option> elements.*
model | `object` | *Get model selected (Output)*
selected | `object` | *Set select value by track (Input).*
placeholder | `string` | *Text into placeholder.*
disabled | `boolean` | *If required disable the component is marked as true.*

##How to contribute

All contributions are very welcome, We love it. There are several ways to help out:

- Create an [issue](https://github.com/Modulr/angular-select2/issues) on GitHub, if you have found a bug
- Write test cases for open bug issues
- Write patches for open bug/feature issues, preferably with test cases included
- Contribute to the documentation

There are a few guidelines that we need contributors to follow so that we have a chance of keeping on top of things.

If you want to making changes Better avoid working directly on the `master` branch, to avoid conflicts if you pull in updates from origin, so, if make your contribution under the branch [`dev`](https://github.com/Modulr/angular-select2/tree/dev), into folder `src/`.

##Community

- Implementation help may be found at Stack Overflow (tagged [`angular-select2`](http://stackoverflow.com/questions/tagged/angular-select2)).

##Creators

[@AlfredoBarronC](https://twitter.com/AlfredoBarronC)

## Copyright and license

Code and documentation (c) Copyright 2015 Modulr. Code published under [license MIT](https://github.com/Modulr/angular-select2/blob/dev/LICENSE)