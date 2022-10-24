# OE CSS (newblue)

The "newblue" CSS repository allows for the development of OpenEyes UI(X) independently of other OpenEyes development work. This is achieved through iDG (a frontend UX prototyping site). ("newblue" started as a moniker for the major v3 UI development work and it just stuck.)

## Concept

* Create a clean, elegant UI(X) that is easy to use
* Minimise visual clutter without losing data clarity
* Present data in a consistent and efficient way to better assist clinical tasks.

## Browser support

* Chrome > 88
* Edge > 88
* Safari > 14.1

## JS hooks

* CSS classes used only as JS hooks (i.e. not being used by CSS to style anything) should be prefixed with `js-`.

## Opinionated SCSS guides

Basically, follow best practices...

* Try to keep selectors short and shallow.
* Avoid ID's for styling. It avoids specificity issues (although, some top level elements do - for historical reasons)
* Use lower-case for classnames, with words separated by a hyphen. (e.g. `.btn-dropdown`)
* Generally, try and use a two level object orientated approach. 
* Generally use semantic, descriptive classnames that hint at their function.
* Avoid qualifying class names with type selectors e.g. `div.myclass` (Unless you want the class to be bound to a specific DOM element)
* Never use `!important` (unless you really, really have too...)


## Iconography

* Event icons must be 76px x 76px, and named correctly.
* Eyedraw icon (doodles) must be 32px x 32px, and named correctly.
* SVGs are used in a few different flavours, see source for examples.

## Please do not use inline styles for adjusting styling

**Why not?** For the following reasons:

1. Inline DOM styling is problematic with theming
2. Responsive layout (UI responsiveness is highly bespoke)
3. UI consistency (consistent data presentation has many, many benefits)
4. Unnecessary, somewhere in OE there is possibly a UI solution already created!
5. Flagging up UI issues with the CSS helps to improve the overall UI across the board

_(To be clear, we are not talking about JS positional stuff, but this does include z stacking which does need considering globally)_

### Finally...

The smallest supported  width is 1200px, with the UIX being tailored to run on handheld tablets, as well as on super-wide displays. 



