# harp-bootstrap-sass

> Bootstrap for Sass, ready to roll.

## Dependencies

* [NodeJS](http://nodejs.org/) – _Server-side JavaScript runtime_
* [Harp](http://harpjs.com/) – _The static web server with built-in preprocessing_

## Install

To install Bootstrap in Sass, run the following command from the root of your Harp project:

```bash
harp install bootstrap-sass
```

Your project will look something like this…

```
myproject/                     <-- Your project root (or public dir if in framework-mode)
  |- components/               <-- Harp puts components here
  |   +- harp-bootstrap-sass/  <-- Where this lib gets installed
  |       …
  |- main.scss                 <-- Where you reference Bootstrap for Sass 
  +- index.jade                <-- Where you reference main.css
```

## Link

Now, from within a `.scss` file in your project, you can `@import` Bootstrap for Sass:

```less
@import "components/harp-bootstrap-sass/scss/bootstrap";
```

Or, just a portion of Bootstrap:

```less
@import "components/harp-bootstrap/scss/variables";
@import "components/harp-bootstrap/scss/mixins";
@import "components/harp-bootstrap/scss/grid";
```

## Resources

* [Harp documentation](http://harpjs.com/docs)
* [Sass documentation](http://sass-lang.org)
* [Bootstrap documentation](http://getbootstrap.com)

## License

This component is [Bootstrap for Sass](https://github.com/thomas-mcdonald/bootstrap-sass), which is Copyright © 2013 Twitter, Inc. under [the Apache 2.0 licensed](https://github.com/twbs/bootstrap/blob/master/LICENSE).