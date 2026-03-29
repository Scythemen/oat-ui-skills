# Button

Demo: https://oat.ink/demo/#button

`<button>` is styled by default, `<a>` needs `.button` class.

## Basic Buttons

```html
<button>Default</button>
<button data-variant="primary">Primary</button>
<button data-variant="secondary">Secondary</button>
<button data-variant="danger">Danger</button>
```

## Style Variants

```html
<button class="outline">Outline</button>
<button class="ghost">Ghost</button>
```

## Sizes

```html
<button class="small">Small</button>
<button class="large">Large</button>
```

## States

```html
<button disabled>Disabled</button>
```

## Link Buttons

```html
<a class="button" href="#">Link Button</a>
<a class="button outline" href="#">Outline Link</a>
```

## Button Groups

```html
<menu class="buttons">
  <li><button class="outline">Left</button></li>
  <li><button class="outline">Center</button></li>
  <li><button class="outline">Right</button></li>
</menu>
```

## Complete Example

```html
<article class="card">
  <header>
    <h3>Confirm Action</h3>
    <p>Please confirm you want to proceed.</p>
  </header>
  <footer class="hstack">
    <button class="outline">Cancel</button>
    <button data-variant="danger">Confirm Delete</button>
  </footer>
</article>
```
