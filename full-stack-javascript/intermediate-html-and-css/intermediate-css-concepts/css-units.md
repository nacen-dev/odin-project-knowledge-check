# CSS Units

## Absolute Units

Absolute units are those that are always the same in any context. px is an absolute unit because the size of a pixel doesn’t change relative to anything else on the page. In fact, px is the only absolute unit you should be using for web projects. The rest of them make more sense in a print setting because they are related to physical units such as in (inch) and cm (centimeter).

## Relative Units

Relative units are units that can change based on their context. There are several of them that you are likely to encounter and want to use.

### em and rem

em and rem both refer to a font size, though they are often used to define other sizes in CSS. You’ll see both of them often so we’re going to explain both, but as a rule-of-thumb, prefer rem.

1em is the font-size of an element (or the element’s parent if you’re using it to set font-size). So, for example, if an element’s font-size is 16px, then setting its width to 4em would make its width 64px (16 \* 4 == 64).

1rem is the font-size of the root element (either :root or html). The math works the same with rem as it did with em, but without the added complexity of keeping track of the parent’s font size. Relying on em could mean that a particular size could change if the context changes, which is very likely not the behavior you want.

Using a relative size like rem to define font sizes across your website is recommended. Many browsers allow users to change the base font-size to increase readability. If at all possible, it is advisable to respect user’s wishes with regards to font size. You’ll learn more about this from the reading assignments.

### Viewport Units

The units vh and vw relate to the size of the viewport. Specifically, 1vh is equal to 1% of the viewport height and 1vw is equal to 1% of the viewport width. These can be useful any time you want something to be sized relative to the viewport, examples including full-height heroes, full-screen app-like interfaces.

## Knowledge Check

### Why would you want to use em or rem for font-size instead of px?

Because these units are relative units which can change depending on the context. For example you can set the font size to a rem unit and you can have a media query that changes the html font size so it the font size can adapt.

### What are some instances where you might want to use vh and vw

These are useful when you want something to be sized relative to the viewport like full screen app interfaces

### What are some instances where you might want to use px instead of a relative unit?

If you do not want a value to change depending on the context but rather have it as a static value, mostly for anything other than font size.
