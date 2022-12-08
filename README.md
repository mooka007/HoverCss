# HoverCss


A collection of CSS3 powered hover effects to be applied to links, buttons, logos, SVG, featured images and so on. Easily apply to your own elements, modify or just use for inspiration. Available in CSS, Sass, and LESS.

## Contents
- [Download/Install](#downloadinstall)
- [How To Use](#how-to-use)
    - [A. Copy and Paste an Effect](#a-copy-and-paste-an-effect)
    - [B. Reference Hover.css](#b-reference-hovercss)
    - [A Note on the display property](#a-note-on-the-display-property)
    - [Using Icon Effects](#using-icon-effects)
- [What's Included?](#whats-included)
    - [css](#css)
    - [scss/less](#scssless)
    - [Other](#other)
- [Browser Support](#browser-support)
- [Using Grunt for Development](#using-grunt-for-development)
- [Using Sass/LESS for Development](#using-sassless-for-development)
    - [_hacks](#\_hacks)
    - [_mixins](#\_mixins)
    - [_options](#\_options)

## How To Use
Hover.css can be used in a number of ways; either copy and paste the effect you'd like to use in your own stylesheet or reference the stylesheet. Then just add the class name of the effect to the element you'd like it applied to.

### A. Copy and Paste an Effect
If you plan on only using one or several effects, it's better practice to copy and paste an effect into your own stylesheet, so a user doesn't have to download `hover.css` in its entirety.

Assuming you want to use the Grow effect:

1. Download Hover.css
2. In `hover.css`, find the Grow CSS (each effect is named using a comment above it):

    ```css
    /* Grow */
    .hvr-grow {
        display: inline-block;
        vertical-align: middle;
        transform: translateZ(0);
        box-shadow: 0 0 1px rgba(0, 0, 0, 0);
        backface-visibility: hidden;
        -moz-osx-font-smoothing: grayscale;
        transition-duration: 0.3s;
        transition-property: transform;
    }

    .hvr-grow:hover,
    .hvr-grow:focus,
    .hvr-grow:active {
        transform: scale(1.1);
    }
    ```
3. Copy this effect and then paste it into your own stylesheet.
4. In the HTML file which you'd like the effect to appear, add the class of `.hvr-grow` to your chosen element.

Example element before applying Hover.css effect:

```html
<a href="#">Add to Basket</a>
```

Example element after applying Hover.css effect:

```html
<a href="#" class="hvr-grow">Add to Basket</a>
```