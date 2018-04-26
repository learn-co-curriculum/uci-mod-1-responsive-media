# Responsive Media

## Overview

In this lesson we will look at a strategy for making our media content responsive.

## Objectives

1. Adjust media sizing to be responsive.

## Adjusting Media For Responsive Layouts

> “You must be shapeless, formless, like water. When you pour water in a cup, it becomes the cup. When you pour water in a bottle, it becomes the bottle. When you pour water in a teapot, it becomes the teapot. Water can drip and it can crash. Become like water my friend.”
> -Bruce Lee

Using percent (%) measurements on our media allows them to fluidly fill the size
of their container. In most cases, our media is contained within the columns and
rows of our layouts.

```css
img, form, input, table, video, audio, iframe {
  width: 100%;
  max-width: 100%;
}
```

Here we set our images, forms, inputs, tables, videos, audio elements, and
iframes all to expand `width: 100%;` setting them to be as wide as the parent
they are inside of. Then using `max-width: 100%;` prevents them from getting any
larger than their parent.

Using both these properties will ensure that they scale fluidly in all browsers.
Having them fill their columns allows us to write fewer media queries overall as
they will squish and expand until we set a fixed size for their parent elements.
This also allows us to focus sizing the parent element of media content, which
will often be a column of sibling elements.  

Consider a website like [Instagram](instagram.com): each photo being displayed
to a user shares a 'column' of content - a username, the photo, likes, comments;
all fit into the width of a 'card' on the page. If the card shrinks or expands
in size, the photo will too. Users on different sized screens will see a web
page that is _slightly_ different, but at all sizes, the content looks good and
is nearly consistent.

## Summary

We can set our media to `width: 100%; max-width: 100%;` to give them flexible
fluid widths that will expand to the size of their parent. This allows us to
write fewer media queries as they will resize to accommodate the device
automatically in most cases.

## Resources

- [Responsive Media Content - Code Example](http://jsfiddle.net/flatiron_school/HP6A3/1/)

<p class='util--hide'>View <a href='https://learn.co/lessons/responsive-media'>Responsive Media</a> on Learn.co and start learning to code for free.</p>
