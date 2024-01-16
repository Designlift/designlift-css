# Designlift CSS
Design for web with just a *few* classes. This simple design system in CSS is focused on consistency, speed, and ease of use.

We wanted to build a super-simple design system that was easy to pick up and hard to get wrong. You don't have to know CSS to use it, and it works great to get an web idea off the ground quickly. It's also easy to build upon with other frameworks and libraries.

## Concepts
Here are some concepts we followed to make it easier to get right:
- Minimal classes and documentation so it's easy to learn.
- Follow well-known design and interaction patterns. Design for 80% of use cases. 
- All styles derived from some base settings which includes colors, fonts, and scale.
- Make the defaults look good. Make it look better easily.
- Modify appearance with a class.
- Responsive without media queries.
- Flexible, but not comprehensive and extensive.
- Make it easy to build upon using other frameworks and libraries.

## Getting Started

### Installation

```
npm add designlift-css
import "designlift-css/package/src/styles/index.css";
```

### Theme
Set the theme of design using the following template and then import after `index.css`.

```
:root {

  /* Foundation */
  --max-font-size: 2rem;
  --min-font-size: 1rem;
  --base-font-size: 1rem;
  --root: 4px;
  --scale: 1.44;
  --rounding: var(--root);
  --alignment: baseline;
  
  /* Layout */
  --border-width: 1px;
  --border-style: solid;
  --element-padding: var(--sm);
  --element-radius: var(--md);
  --element-gap: var(--md);
  --element-shadow: 0 0 var(--md) var(--xs) var(--shadow-color);
  --margin: var(--sm);
  --frame-padding: var(--xl);
  --frame-radius: var(--xl);
  --frame-gap: var(--xl);
  --frame-shadow: 0 0 var(--xl) var(--xs) var(--shadow-color);
  --frame-margin: var(--xl);

  /* Colors */
  --base-text-color: #555;
  --base-heading-color: #333;
  --base-surface-color: #ddd;
  --base-border-color: #ccc;
  --base-hover-color: #eee;
  --highlight-heading-color: #fff;
  --highlight-text-color: #ddd;
  --highlight-surface-color: #222;
  --highlight-border-color: #444;
  --accent-heading-color: #333;
  --accent-text-color: #555;
  --accent-surface-color: #fff;
  --accent-border-color: #fff;
  --action-heading-color: #fff;
  --action-text-color: #fff;
  --action-surface-color: #ff0000;
  --action-border-color: #ff0000;
  --action-hover-color: #ff4444;
  --transparent-color: rgba(0,0,0,0);
  --shadow-color: rgba(0,0,0,0.1);

  /* Interactions */
  --action-base-transition: 0.1s;
  --action-base-position: translate(0, -0.25rem);
  --action-hover-position: translate(0, -0.25rem);
  --action-base-shadow: 0 0.25em 0 0 #cc0000;
  --action-hover-shadow: 0 0.25em 0 0 #dd0000;
  --action-active-shadow: 0 0.05em 0 0 #cc0000;
  --action-active-position: translate(0, 0);
  --element-hover-shadow: 0 0 var(--md) var(--md) var(--shadow-color);
  --element-transition: box-shadow 0.3s ease-in-out;
  --frame-hover-shadow: 0 0 var(--xl) var(--xl) var(--shadow-color);
  --frame-transition: box-shadow 0.3s ease-in-out;

  /* Typography */
  --base-font-family: 'Inter Variable', sans-serif;
  --heading-font-family: 'Inter Variable', sans-serif;
  --accent-font-family: 'Inter Variable', sans-serif;
  --base-font-style: italic;
  --heading-font-style: bold italic;
  --measure: 66ch;
  --line-height: var(--scale);

  /* Other */
  --details-icon-closed: '';
  --details-icon-open: '';
  --grid-min-size: var(--w-xxl); /* Adjust to fit scale */
  --grid-max-size: 1fr;
}
```

Each page can be layed out by following the process below:

### Layout
1. Establish layout heirarchy by designating important groups of content as frames using the `frame` class. Frames give content visual weight.
2. Determine the direction elements should flow within any particular element with the `horizontal`, `vertical`, `stack`, or `grid`  class.
3. Arrange content with `around`, `between`, `split`, `start`, `center`, or `end` classes.
4. Position text with `left`, `center`, or `right` classes.

### Style
1. Use color to emphasize text or frames with the `accent`, `action`, or `highlight` class.
2. Style frames and elements with `background`, `border`, `gap`, `padding`, `radius`, `round` and `shadow` classes.
3. Emphasize primary calls to action with the `primary`, `secondary`, or `default` on button and link elements.

### Scale
- Set the size of text with the `xxs`, `xs`, `sm`, `md`, `lg`, `xl`, `xxl`, `xxxl` classes.
- Set the height of elements with `h-xxs`, `h-xs`, `h-sm`, `h-md`, `h-lg`, `h-xl`, `h-xxl`, `h-xxxl` classes.
- Set the width of elements with `w-xxs`, `w-xs`, `w-sm`, `w-md`, `w-lg`, `w-xl`, `w-xxl`, `w-xxxl` classes.

### Advanced
- Make an element fill the page with the `fill` class.
- Grow to fill remaining space with the `grow` class.
- Make an element scrollable with the `scroll` class.
- Make an element sticky with the `stick` class.
- Make an element animate between states with the `animation` class.


## Examples

```
<section class="frame padding vertical center gap highlight">
  <hgroup>
    <h2 class="xxl">Prepare for <span class="action">liftoff</span></h2>
    <p>Build websites from a launchpad</p>
  </hgroup>
  <div class="horizontal gap">
    <a href="#" class="primary">Launch</a>
    <a href="#" class="secondary">Launch</a>
  </div>
</section>
```
