# Utilities

CSS utility classes for layout, spacing, alignment, and text. No component required — just add the class.

## Layout Helpers

### Horizontal Stack (`.hstack`)

Flex row with centered items, wrapping, gap, and zeroed child margins.

```html
<footer class="hstack">
  <button class="outline">Cancel</button>
  <button>Save</button>
</footer>
```

### Vertical Stack (`.vstack`)

Flex column with gap.

```html
<div class="vstack">
  <label>Name</label>
  <input type="text">
  <label>Email</label>
  <input type="email">
</div>
```

## Flex Utilities

| Class | CSS |
|-------|-----|
| `.flex` | `display: flex` |
| `.flex-col` | `flex-direction: column` |
| `.items-center` | `align-items: center` |
| `.justify-center` | `justify-content: center` |
| `.justify-between` | `justify-content: space-between` |
| `.justify-end` | `justify-content: flex-end` |

### Examples

```html
<!-- Centered content -->
<div class="flex items-center justify-center" style="height: 200px">
  <p>Centered</p>
</div>

<!-- Space between -->
<header class="flex justify-between items-center">
  <span>Logo</span>
  <button>Menu</button>
</header>

<!-- Right-aligned actions -->
<div class="flex justify-end">
  <button>Next</button>
</div>
```

## Gap Utilities

| Class | Value |
|-------|-------|
| `.gap-1` | `var(--space-1)` |
| `.gap-2` | `var(--space-2)` |
| `.gap-4` | `var(--space-4)` |

`.hstack` and `.vstack` already include `gap: var(--space-3)`. Use explicit `.gap-*` classes to override.

```html
<div class="flex gap-2">
  <span class="badge">A</span>
  <span class="badge">B</span>
</div>
```

## Margin Utilities

### Margin Block Start (`.mt-*`)

| Class | Value |
|-------|-------|
| `.mt-2` | `var(--space-2)` |
| `.mt-4` | `var(--space-4)` |
| `.mt-6` | `var(--space-6)` |

### Margin Block End (`.mb-*`)

| Class | Value |
|-------|-------|
| `.mb-2` | `var(--space-2)` |
| `.mb-4` | `var(--space-4)` |
| `.mb-6` | `var(--space-6)` |

```html
<h2 class="mb-4">Section Title</h2>
<p class="mb-2">First paragraph.</p>
<p class="mt-6">With extra top margin.</p>
```

## Padding

| Class | Value |
|-------|-------|
| `.p-4` | `var(--space-4)` |

```html
<div class="p-4">Padded container</div>
```

## Width

| Class | CSS |
|-------|-----|
| `.w-100` | `width: 100%` |

```html
<button class="w-100">Full-width button</button>
```

## Text Alignment

| Class | CSS |
|-------|-----|
| `.align-left` | `text-align: start` |
| `.align-center` | `text-align: center` |
| `.align-right` | `text-align: end` |

## Text Color

| Class | Applies |
|-------|---------|
| `.text-light` | `color: var(--muted-foreground)` |
| `.text-lighter` | `color: var(--faint-foreground)` |

```html
<p class="text-light">Muted secondary text.</p>
<span class="text-lighter">Faint hint text.</span>
```

## `.unstyled`

Removes default list-style, text-decoration, and padding from `<ul>`, `<ol>`, and `<a>` elements.

```html
<ol class="unstyled hstack">
  <li><a href="/" class="unstyled">Home</a></li>
  <li><a href="/about" class="unstyled">About</a></li>
</ol>
```

## Combining Utilities

All utilities compose freely:

```html
<!-- Card-like layout using only utilities -->
<div class="vstack gap-2 p-4">
  <h3 class="mb-2">Title</h3>
  <p class="text-light mb-4">Description text.</p>
  <div class="flex justify-end gap-2">
    <button class="outline">Cancel</button>
    <button>Confirm</button>
  </div>
</div>
```
