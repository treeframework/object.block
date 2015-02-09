# Block

The Block object simply stacks an image on top of some text content.

This incredibly frequently occurring design pattern is now wrapped up in a
simple, reusable, configurable abstraction.

## Dependencies

The Block object depends on two other modules:

* [settings.defaults](https://github.com/treeframework/settings.defaults)
* [tools.functions](https://github.com/treeframework/tools.functions)

If you install the Block object using Bower, you will get these dependencies at
the same time. If not using Bower, please be sure to install and `@import` these
dependencies in the relevant way.

## Installation

The recommended installation method is Bower, but you can install the Block
module via npm, Git Submodule, or copy and paste.

### Install using Bower:

```sh
$ bower install tree-block --save
```

### Install using npm:

```sh
$ npm install tree-block --save
```


Once installed, `@import` into your project in its Object layer:

```scss
@import "bower_componenets/tree-block/object.block";
```

### Install as a Git Submodule:

```sh
$ git submodule add git@github.com:treeframework/object.block.git
```

Once installed, `@import` into your project in its Objects layer:

```scss
@import "object.block/object.block";
```

### Install via file download

The least recommended option for installation is to simply download
`_object.block.scss` into your project and `@import` it into your project in its
Objects layer.

## Usage

Basic usage of the Block object uses the required classes:

```html
<div class="block">
    <img class="block__img" src="/path/to/image.png" alt="" />
    <div class="block__body">
        <p>Text-like content goes here.</p>
    </div>
</div>
```

The only valid children of the `.block` node are `.block__img` and
`.block__body`.

## Options

Other, optional classes can supplement the required base classes:

* `.block--flush`: remove the space between the stacked image- and text-content.
* `.block--[tiny|small|large|huge]`: alter the spacing between the stacked
  image- and text-content.
* `.block--[center|right]`: align both the image- and text-content.

For example:

```html
<div class="block  block--small  block--center">
    <img class="block__img" src="/path/to/image.png" alt="" />
    <div class="block__body">
        <p>Text-like content goes here.</p>
    </div>
</div>
```

## Credits

* **[inuitcss](https://github.com/inuitcss)** Powerful, Sass-based, OOCSS
framework designed with scalability and performance in mind.
