# SSD2850 - Assignment 04

### Group Members
* Ethan
* Pawel
* Poul

## Project folder Structure

```text
assets/
styles/
    components/
      _button.css
      _card.css
      _navbar.css
    utilities/
    base.css
scripts/
index.html
```

---


# Style Guide

Use [BEM](https://en.bem.info/methodology) when styling components

For colours, pick from [TailwindCSS Colors](https://tailwindcss.com/docs/colors#Colors),
find the corresponding CSS variable in [styles/colours.css](styles/colours.css) and use that.
```css
<selector> {
  color: var(--color-red-500);
}
```
Use specific, one-off colour values sparingly. If you need to use a custom colour value
in multiple places, append a new CSS variable to [styles/colours.css](styles/colours.css) in the `:root` block.

```css
:root {
    /* ... */
    --color-something: #aaff00;
}
```

## Examples

### Example: Button Component

```html
...
<button class="button button--primary">
  Submit
</button>
...
```

```css
/* _button.css */
.button {
  display: inline-flex;
  align-items: center;
  border-radius: 0.5rem;
  padding: 0.5rem 1rem;
}

.button--primary {
  font-weight: bold;
  background-color: var(--color-primary);
}
```
