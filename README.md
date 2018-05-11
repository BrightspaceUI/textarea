# d2l-textarea
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/BrightspaceUI/textarea)
[![Bower version][bower-image]][bower-url]
[![Build status][ci-image]][ci-url]

[Polymer](https://www.polymer-project.org)-based web component for D2L text area.

![screenshot of d2l-textarea autogrowing](/d2l-textarea.gif?raw=true)

For further information on this and other Brightspace UI components, see the docs at [ui.developers.brightspace.com](http://ui.developers.brightspace.com/).

## Installation

`d2l-textarea` can be installed from [Bower][bower-url]:

```shell
bower install d2l-textarea
```

## Usage

Include the [webcomponents.js](http://webcomponents.org/polyfills/) "lite" polyfill (for browsers who don't natively support web components), then import the component as needed:

```html
<head>
  <script src="../webcomponentsjs/webcomponents-lite.js"></script>
  <link rel="import" href="../d2l-textarea/d2l-textarea.html">
</head>
```

Then use the `<d2l-textarea>` custom element in your application.

```html
<d2l-textarea name="myInput" value="input value"></d2l-textarea>
```

Many of the same attributes from native [`<textarea>` are available](https://developer.mozilla.org/en/docs/Web/HTML/Element/textarea):

```html
<d2l-textarea disabled></d2l-textarea>
```

These attributes may also be used:
* `no-border` removes border styling from the text area.
* `hover-styles` applies (square) hover styling to the text area.

![screenshot of no-border and hover-styles attributes](/no-border_hover-styles.gif?raw=true)
````html
<d2l-textarea no-border hover-styles></d2l-textarea>
````

## Developing, Testing and Contributing

After cloning the repo, run `npm install` to install dependencies.

If you don't have it already, install the [Polymer CLI](https://www.polymer-project.org/2.0/docs/tools/polymer-cli) globally:

```shell
npm install -g polymer-cli
```

To start a [local web server](https://www.polymer-project.org/2.0/docs/tools/polymer-cli-commands#serve) that hosts the demo page and tests:

```shell
polymer serve
```

To lint ([eslint](http://eslint.org/) and [Polymer lint](https://www.polymer-project.org/2.0/docs/tools/polymer-cli-commands#lint)):

```shell
npm run test:lint
```

To run unit tests locally using [Polymer test](https://www.polymer-project.org/2.0/docs/tools/polymer-cli-commands#tests):

```shell
polymer test --skip-plugin sauce
```

To lint AND run local unit tests:

```shell
npm test
```

[bower-url]: http://bower.io/search/?q=d2l-textarea
[bower-image]: https://badge.fury.io/bo/d2l-textarea.svg
[ci-url]: https://travis-ci.org/BrightspaceUI/textarea
[ci-image]: https://travis-ci.org/BrightspaceUI/textarea.svg?branch=master
