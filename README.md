# Trillo - A Flexbox Project

This is the second project from the [Jonas Schmedtmann's Advanced CSS and Sass course.](https://www.udemy.com/advanced-css-and-sass/ "Udemy | Advanced CSS and Sass: Flexbox, Grid, Animations and More!") Main goal of this project was to build a responsive landing page by using the **Flexbox** CSS layout method.


## Table of Contents

- [Flexbox](#flexbox)
- [CSS custom properties (variables)](#css-custom-properties-variables)
- [SVG icons vs. icon fonts](#svg-icons-vs-icon-fonts)


## Flexbox

Flexbox is a one-dimensional layout method for laying out items in rows or columns. The main idea behind the flexbox is to give the container, a parent element with `display: flex` property the ability to expand children elements to fill available free space or shrink them to prevent overflow, and thus best utilize the available space. Also, children elements order can easily be rearranged by using the CSS `order` property.

As stated on the [MDN Flexbox Page](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox), some of the best use cases of flexbox layout are:

> - Vertically centering a block of content inside its parent.
> - Making all the children of a container take up an equal amount of the available width/height, regardless of how much width/height is available.
> - Making all columns in a multiple-column layout adopt the same height even if they contain a different amount of content.

Flexbox is supported in all major browsers except IE 9 and lower. *[See browser support on caniuse.com website.](https://caniuse.com/?search=flexbox "Can I use flexbox?")*

*Browser support, December 2020:*

![Flexbox browser support December 2020](img/readme/can-i-use-flexbox.png "Browser support")


## CSS custom properties (variables)

>Custom properties (sometimes referred to as CSS variables or cascading variables) are entities defined by CSS authors that contain specific values to be reused throughout a document.
*Source: [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties#Values_in_JavaScript "Using CSS custom properties (variables)")*

They are usually defined in the `:root` CSS pseudo-class which represents the `<html>` element and is identical to the selector `html`, except that its specificity is higher. *[See more on MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/:root)*

![Defining CSS custom properties (variables) in `:root` element](img/readme/css-variables-root.png "Defining CSS variables")

We can then easily access those CSS variables by using the `var()` function: `color: var(--color-primary);`

Main reasons why to use native CSS instead of SASS variables:

> You can use them **without the need of a preprocessor**.
> **They cascade.** You can set a variable inside any selector to set or override its current value.
> When their values change (e.g. media query or other state), **the browser repaints as needed**.
> You can access and **manipulate them in JavaScript**.
*Source: [CSS-TRICKS](https://css-tricks.com/difference-between-types-of-css-variables/ "What is the difference between CSS variables and preprocessor variables?")*

Another interesting article on codyhouse.co: [Why we prefer CSS Custom Properties to SASS variables](https://codyhouse.co/blog/post/css-custom-properties-vs-sass-variables).

CSS variables are not supported in IE browsers. *[See browser support on caniuse.com website.](https://caniuse.com/?search=variables)*

*Browser support, December 2020:*

![CSS variables browser support December 2020](img/readme/can-i-use-css-variables.png "Browser support")


## SVG icons vs. icon fonts

