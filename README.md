# Tachygrid

A small grid module for Tachyons CSS.

## What’s this?

[Tachyons](http://tachyons.io) is an atomic CSS framework which comes with a flexbox module, but no CSS grid. Tachygrid provides just that, along with some opinionated layouts (i.e. halves, thirds, quarters, and two main/sidebar combinations, covering 99.99% of my layout requirements).

## Namespacing

All Tachygrids classes are namespaced c-, so you can use it with Tachyons with no problems. The example references a copy of Tachyons 4.10.0 and an additional file with the grid CSS.

## Usage

Grid uses inheritance, while Tachyons doesn’t. Grid will probably make you rethink how you use CSS, and even Tachyons. I’ve used Tachyons for five years, so I’m a bit inbetween.

However, it’s relatively simple. Apply _all_ relevant classes to the parent and the browser will do the heavy grid elements lifting for you. See the index.html file for examples.

## Widths

Tachygrids respects Tachyons’ media query suffixes (i.e. -ns, -m and -l). In an ideal world, you wouldn’t need these with grid as you’d like to _suggest_ something like _each item in the grid is ideally 10rem wide, , minimum 5rem, maximum 20rem – arrange elements accordingly_, which you sort of can with minmax. However, browser support isn’t quite there yet, so I’m using viewport queries.

It’s still pretty flexible. For example, you can easily set a grid that stacks elements by default, arranges them in halves in the medium media query and uses thirds in the large query.
