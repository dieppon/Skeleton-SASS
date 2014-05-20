# One SASSy Skeleton

[Skeleton](http://www.getskeleton.com)'s responsive CSS grid rocks. But some of us don't like muddling up our clean semantic HTML markup with grid framework classes. The value of CSS is in letting you separate presentation and content, so a good CSS grid framework will let you use it completely in your own site's CSS, by applying grid widths to your pre-existing CSS classes and selectors.

Skeleton-SASS is a one-to-one translation of the classes in Skeleton's grid framework, but remixed as SASS mixins. Instead of giving a div a class of `six columns`, inside your own CSS specifying the div you'd simply include the mixin `+columns(6)`.

You can still use the pre-define classes to quickly build the grid by using just 2 includes `column-list` and `offset-list`.

The other big advantage of Skeleton-SASS is that the actual grid widths are only calculated at compile-time. This means that your page width, number of columns, and margin sizes are all easily tweakable if you want to mix things up —- say, switch from a 16-column grid to a 24-column, or bump everything up to 1024px instead of 960px.

The @media queries have been *mixin-fied* for a clear implementation throughout your project using , using `respond-to` simple names such as *desktop, tablet* or *mobile*.

###Usage

1. Add this partial to your project.

2. Define *$base-width, $tablet-width, $mobile-portrait-width,$mobile-landscape-width, $num-columns, $margin, $border-width* with the rest of your varibles.

3. Use the mixins on your layout SCSS to quickly create a responsive grid.