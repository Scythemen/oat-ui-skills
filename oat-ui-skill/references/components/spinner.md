# Spinner

`aria-busy="true"` activates spinner, with size customization.

## Basic Usage

```html
<div aria-busy="true"></div>
```

## Size Variants

```html
<div aria-busy="true" data-spinner="small"></div>
<div aria-busy="true" data-spinner="large"></div>
```

## Overlay Mode

```html
<article class="card" aria-busy="true" data-spinner="large overlay">
  <header><h3>Loading...</h3><p>Please wait</p></header>
  <p>Content area</p>
</article>
```

## Spinner in Button

```html
<button aria-busy="true" data-spinner="small" disabled>Loading...</button>
```

## With Form

```html
<form>
  <label>
    Username
    <input type="text" id="username" placeholder="Enter username">
  </label>
  <button aria-busy="true" data-spinner="small" disabled>Submitting...</button>
</form>
```

## Complete Loading Example

```html
<article class="card" aria-busy="true" data-spinner="large overlay">
  <header>
    <h3>Data Loading</h3>
    <p>Fetching user information...</p>
  </header>
  <div>
    <div style="display: flex; gap: var(--space-2); margin-bottom: var(--space-2);">
      <div role="status" class="skeleton line" style="width: 80px;"></div>
      <div role="status" class="skeleton line" style="width: 120px;"></div>
    </div>
    <div role="status" class="skeleton line"></div>
    <div role="status" class="skeleton line" style="width: 60%;"></div>
  </div>
</article>
```

## data-spinner Values

| Value | Description |
|-------|-------------|
| `small` | Small size |
| `large` | Large size |
| `overlay` | Overlay mode (use with `.card`) |
