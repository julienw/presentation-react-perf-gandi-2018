# A Mozilla theme for [Remark](https://remarkjs.com/)

Remark is awesome. I use it all the time for my talks. So I needed a Mozilla
theme with the latest changes.

This theme follows the Mozilla code style as of February 2018. Some colors were
slightly modified for accessibility concerns, as the contrast wasn't good
enough.

All colors are defined as CSS variables for your convenience.

## Fonts
The fonts [Fira Sans](https://github.com/carrois/Fira/),
[Fira Mono](https://github.com/carrois/Fira/) and [Fira Code](https://github.com/tonsky/FiraCode)
are preconfigured, both _regular_ and _bold_ weights. `Fira Code` is used for
code fences but it's easy to switch if you'd rather use `Fira Mono`.

If you want more variants for the fonts, please help yourself and shoot a PR to me!

The fonts are configured with woff2 only. I thought that because I also
specified a fallback, this is fine if some older browser doesn't use it.

Last thing about fonts is I used the latin subset for Fira. This means some
glyphs will be missing, but I don't know more. Feel free to replace them with
the full variant in a PR if you know what's the difference and it is useful.

## Special styles

Some things are already styled for your pleasure:

* `li` have a margin
* `h1` are smaller and bold
* `img` can't be bigger than the width, and highe than 45% of the page
* `em` (generated with `_` in markdown) are orange. `strong` are _not_ styled
  yet (PR welcome!)
* `a` have a paler blue for accessibility
* The text is bigger than what remark does by default.

## Pre-defined classes

I defined some classes for my taste. You can find:

* `cover` for the first slide, makes things bigger, and put the `Mozilla` logo
  in a different place.
* `smaller`: this, obviously, makes the text smaller. This is useful if you have a
  slide with more content than the others.
* `smallest`: if you need something even smaller. Note you can also combine
  them.
* `float-left` and `float-right`: this is obvious

## Pre-defined colors

```
:root {
  --light-blue: rgb(0, 150, 221);
  --lighter-blue: rgb(0, 170, 245);
  --navy-blue: rgb(0, 33, 71);
  --light-orange: rgb(255, 149, 0);
  --orange: rgb(230, 96, 0);
  --red: rgb(193, 56, 50);
  --yellow: rgb(255, 203, 0);
  --gecko-green: rgb(111, 190, 74);
  --grey-coal: rgb(77, 78, 83);
  --light-grey: rgb(208, 211, 212);
}
```
