# skeletor.css
![skeletor](http://stream1.gifsoup.com/view2/1632356/smilin-skeletor-o.gif)
* That's who you're going to meet when writing unmantainable CSS.

## Motivation

### TL;DR

* a down-to-earth minimal set up for website/app development
* no colors, no typefaces, no design decisions made for you
* 100% modular
* easily configurable through variables
* *(hopefully)* promoting sane architecture, writing clean and maintainable CSS :sunny:
* built in [Stylus](https://github.com/learnboost/stylus)

### Long story
Most of front-end frameworks ([Pure](http://purecss.io/), [Bootstrap](http://getbootstrap.com/), [Foundation](http://foundation.zurb.com/), etc.) come with predefined styles &mdash; typefaces, color palette as well as built-in components. While those are great for rapid prototyping and enabling people who are less front-end savvy they can potentially introduce a lot of unnecessary code. When mishandled months later one might wonder why CSS takes 10 seconds to load and how is it possible to have several thousand lines of CSS for a simple website. 

I like simplicity. I'm inspired by [Unix Philosophy](http://en.wikipedia.org/wiki/Unix_philosophy#Eric_Raymond.E2.80.99s_17_Unix_Rules) and [the modular ecosystem](https://www.npmjs.org/) around Node.js.

I believe it's better to have a simple, bare bones set of modules (aka files that will be imported or not) to build on, rather than a library that tries to do it all.

## Structure

```
├── styl
  └── components
    ├── base.styl
    ├── buttons.styl
    ├── forms.styl
    └── list.styl
  └── globals
    └── _variables.styl
  └── skeletor.styl
```

Intentionally there is no compiled version so you can choose which modules you need or add more to `skeletor.styl` through `@import` rule.

## License
MIT