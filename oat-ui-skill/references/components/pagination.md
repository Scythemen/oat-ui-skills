# Pagination

Reuses Button component with `<nav>` semantics.

## Basic Pagination

```html
<nav aria-label="Pagination">
  <menu class="buttons">
    <li><a href="#" class="button outline small">← Previous</a></li>
    <li><a href="#" class="button outline small">1</a></li>
    <li><a href="#" class="button outline small">2</a></li>
    <li><a href="#" class="button outline small">3</a></li>
    <li><a href="#" class="button outline small">Next →</a></li>
  </menu>
</nav>
```

## Current Page Indicator

Use `aria-current="page"` to mark the current page:

```html
<nav aria-label="Pagination">
  <menu class="buttons">
    <li><a href="#" class="button outline small">← Previous</a></li>
    <li><a href="#" class="button outline small">1</a></li>
    <li><a href="#" class="button small" aria-current="page">2</a></li>
    <li><a href="#" class="button outline small">3</a></li>
    <li><a href="#" class="button outline small">4</a></li>
    <li><a href="#" class="button outline small">Next →</a></li>
  </menu>
</nav>
```

## Ellipsis Pagination (Many Pages)

```html
<nav aria-label="Pagination">
  <menu class="buttons">
    <li><a href="#" class="button outline small">←</a></li>
    <li><a href="#" class="button outline small">1</a></li>
    <li><span class="button outline small" style="cursor: default;">...</span></li>
    <li><a href="#" class="button outline small">10</a></li>
    <li><a href="#" class="button outline small" aria-current="page">11</a></li>
    <li><a href="#" class="button outline small">12</a></li>
    <li><span class="button outline small" style="cursor: default;">...</span></li>
    <li><a href="#" class="button outline small">50</a></li>
    <li><a href="#" class="button outline small">→</a></li>
  </menu>
</nav>
```
