# Block

The `block` object simply stacks an image on top of some text content.

This incredibly frequently occurring design pattern is now wrapped up in a
simple, reusable, configurable abstraction.

## Dependencies

The `block` object depends on two other modules:

* [settings.defaults](https://github.com/treeframework/settings.defaults)
* [tools.functions](https://github.com/treeframework/tools.functions)

If you install the Block object using Bower or npm, you will get these 
dependencies at the same time. If not using Bower or npm, please be sure to 
install and `@import` these dependencies in the relevant way.

## Installation

You can install the `block` module via Bower, npm, or copy and paste.

### Install using Bower:

```sh
$ bower install tree-block --save
```

Once installed, `@import` into your project in its Object layer:

```scss
@import "bower_components/tree-block/object.block";
```

### Install using npm:

```sh
$ npm install tree-block --save
```

### Install via file download

The least recommended option for installation is to simply download
`_object.block.scss` into your project and `@import` it into your project in its
Objects layer.

## Usage

Basic usage of the `block` object uses the required classes:

```html
<div class="o-block">
    <img class="o-block__img" src="/path/to/image.png" alt="" />
    <div class="o-block__body">
        <p>Text-like content goes here.</p>
    </div>
</div>
```

The only valid children of the `.o-block` node are `.o-block__img` and
`.o-block__body`.

## Options

Other, optional classes can supplement the required base classes:

* `.o-block--flush`: remove the space between the stacked image- and text-content.
* `.o-block--[tiny|small|large|huge]`: alter the spacing between the stacked
  image- and text-content.
* `.o-block--[center|right]`: align both the image- and text-content.

For example:

```html
<div class="o-block  o-block--small  o-block--center">
    <img class="o-block__img" src="/path/to/image.png" alt="" />
    <div class="o-block__body">
        <p>Text-like content goes here.</p>
    </div>
</div>
```

## Credits

* **[inuitcss](https://github.com/inuitcss)** Powerful, Sass-based, OOCSS
framework designed with scalability and performance in mind.
