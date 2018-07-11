# A Mozilla theme for [Remark](https://remarkjs.com/)

Remark is awesome. I use it all the time for my talks. So I needed a Mozilla
theme with the latest changes.

This theme follows the Mozilla code style as of June 2018.

All colors are defined as CSS variables for your convenience.

## Fonts
The fonts [Zilla Slab](https://github.com/mozilla/zilla-slab) (including the
"Highlight" version being used for the Mozilla logo) are preconfigured in all
their variants.
The fonts [Fira Mono](https://github.com/carrois/Fira/) and [Fira Code](https://github.com/tonsky/FiraCode)
are also configured for code fences. By default `Fira Code` is used but it's
easy to switch to `Fira Mono` if you prefer it.

The font [Fira Sans](https://github.com/carrois/Fira/) is also preconfigured for
some variangs but not used by default. It's easy to switch by changing
style.css.  

Last thing about fonts is I used the latin subset for Fira. This means some
glyphs will be missing, but I don't know more. Feel free to replace them with
the full variant in a PR if you know what's the difference and it is useful.

## Special styles

Some things are already styled for your pleasure:

* `li` have a margin
* `h1` are smaller and bold
* `img` can't be bigger than the width, and higher than 460px (remember the page
  is then scaled according to the available space, so `460px` is relative to
  this). If you want to add a caption, use the class `with-caption` to set the
  height to 390px.
* `em` (generated with `_` in markdown) are orange. `strong` are _not_ styled
  yet (PR welcome!)
* `a` have some :hover style.
* The text is bigger than what remark does by default.

## Pre-defined classes

I defined some classes for my taste. You can find:

* `cover` for the first slide, makes things bigger, and put the `Mozilla` logo
  in a different place.
* `smaller`: this, obviously, makes the text smaller. This is useful if you have a
  slide with more content than the others.
* `smallest`: if you need something even smaller. Note you can also combine
  them.
* `flex`: sets a `display: flex` on a container. This is useful if you want to
  have some text besides an image.
* `with-caption`: sets slightly smaller `max-height` for images that have a
  caption below.

## Pre-defined colors

```
:root {
  --orange: rgb(240, 93, 52);
  --yellow: rgb(255, 233, 0);
  --grey-coal: rgb(77, 78, 83);
  --blue-green: rgb(34, 156, 178);
}
```
