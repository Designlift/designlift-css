# Designlift
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
### Theme
Set the theme of design in the `theme.css`. Set defaults and go from there, or override the calculated values.

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
