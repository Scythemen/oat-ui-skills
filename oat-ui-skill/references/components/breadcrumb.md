# Breadcrumb

Semantic `<nav>` + `<ol>` structure for navigation paths.

## Basic Structure

```html
<nav aria-label="Breadcrumb">
  <ol class="unstyled hstack">
    <li><a href="/" class="unstyled">Home</a></li>
    <li aria-hidden="true">/</li>
    <li><a href="/products" class="unstyled">Products</a></li>
    <li aria-hidden="true">/</li>
    <li><a href="#" class="unstyled" aria-current="page"><strong>Current Page</strong></a></li>
  </ol>
</nav>
```

## Classes

- `.unstyled` — removes link underlines and default styles
- `.hstack` — horizontal layout
- `aria-current="page"` — marks the current page

## Complete Example

```html
<nav aria-label="Breadcrumb">
  <ol class="unstyled hstack" style="gap: var(--space-1);">
    <li><a href="#" class="unstyled">Home</a></li>
    <li aria-hidden="true" style="color: var(--text-muted);">/</li>
    <li><a href="#" class="unstyled">Documentation</a></li>
    <li aria-hidden="true" style="color: var(--text-muted);">/</li>
    <li><a href="#" class="unstyled" aria-current="page">Components</a></li>
  </ol>
</nav>
```
