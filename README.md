# cb-style-foundation

A SASS library providing basic components and typography for a unified CareerBuilder experience.

**Status:** Still hammering things out!

### Consumption

Install with Bower (from an appropriate repository)

```sh
$ bower install cb-style-foundation
```

Now, import `sass/base` in your main `application.scss`. For example:

```scss
@import 'bower/cb-style-foundation/sass/base';
```

### What's included

At the moment, only uncompiled SASS source files are available for consumption. That means your application will need to perform the precompilation, whether it be through Gulp, Grunt, Rails asset pipeline, etc. Do note that `cb-style-foundation` depends upon [Bourbon](http://bourbon.io/) for basic SASS mixins. Additionally, this library includes its own reset.

The current layout of this library is heavily inspired by [Bitters](http://bitters.bourbon.io/), a wonderful boilerplate of common-sense SASS conventions and structure. Our outline looks a little something like this:

```
dist/
├── ... >> Not yet used
sass/ >> The bulk of the styling itself
├── directives/ >> Mixins and @extend-only selectors, AKA useful functions to build a site with
└── variables/ >> Re-usable color and sizing variables
```

### Future

- Implement build process to compile CSS into `dist` for easy consumption
- Remove `bourbon` dependency
- Build separate `cb-style-grid` library - there is no grid boilerplate in this foundation.
