# harp-bootstrap-sass

> Bootstrap Sass, ready to roll.

## Dependencies

* [NodeJS](http://nodejs.org/) – _Server-side JavaScript runtime_
* [Harp](http://harpjs.com/) – _The static web server with built-in preprocessing_
* [Component](http://component.io) – _Client package management for building better web applications__

## Install

First, install Harp and Component:

```bash
sudo npm install -g harp
sudo npm install -g component
```

To install Bootstrap Sass, run the following commands from the root of your Harp project:

```bash
component install harp/bootstrap-sass
```

Your project will look something like this…

```
myproject/                     <-- Your project root (or public dir if in framework-mode)
  |- components/               <-- Harp puts components here
  |   +- harp-bootstrap-sass/  <-- Where this lib gets installed
  |       …
  |- main.scss                 <-- Where you reference Bootstrap Sass 
  +- index.jade                <-- Where you reference main.css
```

## Link

Now, from within a `.scss` file in your project, you can `@import` Bootstrap Sass:

```less
@import "components/harp-bootstrap-sass/scss/bootstrap";
```

Or, just a portion of Bootstrap:

```less
@import "components/harp-bootstrap/scss/variables";
@import "components/harp-bootstrap/scss/mixins";
@import "components/harp-bootstrap/scss/grid";
```

## Use

Bootstrap Sass for Harp is the same as Bootstrap Sass, save a few differences that are blocked by issue [#231](https://github.com/hcatlin/libsass/issues/231) in libsass: the `img-retina` mixin is not supported, and neither are the Glyphicons partial is not included by default.

## Resources

* [Harp documentation](http://harpjs.com/docs)
* [Sass documentation](http://sass-lang.org)
* [Bootstrap documentation](http://getbootstrap.com)

## License

This component is [Bootstrap Sass](https://github.com/thomas-mcdonald/bootstrap-sass), which is Copyright © 2013 Twitter, Inc. under [the Apache 2.0 licensed](https://github.com/twbs/bootstrap/blob/master/LICENSE).