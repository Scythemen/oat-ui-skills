# Skeleton

Skeleton screen placeholders using `.skeleton` + `role="status"`.

## Basic Usage

```html
<div role="status" class="skeleton line"></div>
<div role="status" class="skeleton box"></div>
```

## Skeleton Types

| Type | Class | Purpose |
|------|-------|---------|
| `.line` | Line | Text line placeholder |
| `.box` | Box | Image or card placeholder |

## User Card Skeleton

```html
<article style="display: flex; gap: var(--space-3);">
  <div role="status" class="skeleton box"></div>
  <div style="flex: 1; display: flex; flex-direction: column; gap: var(--space-1);">
    <div role="status" class="skeleton line"></div>
    <div role="status" class="skeleton line" style="width: 60%;"></div>
  </div>
</article>
```

## Article Card Skeleton

```html
<article class="card">
  <header style="display: flex; gap: var(--space-2);">
    <div role="status" class="skeleton box" style="width: 40px; height: 40px;"></div>
    <div style="flex: 1;">
      <div role="status" class="skeleton line" style="width: 40%;"></div>
      <div role="status" class="skeleton line" style="width: 25%; margin-top: 4px;"></div>
    </div>
  </header>
  <div role="status" class="skeleton line"></div>
  <div role="status" class="skeleton line"></div>
  <div role="status" class="skeleton line" style="width: 75%;"></div>
</article>
```

## Table Skeleton

```html
<div class="table">
  <table>
    <thead>
      <tr>
        <th><div role="status" class="skeleton line" style="width: 60px;"></div></th>
        <th><div role="status" class="skeleton line" style="width: 100px;"></div></th>
        <th><div role="status" class="skeleton line" style="width: 80px;"></div></th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><div role="status" class="skeleton line" style="width: 60px;"></div></td>
        <td><div role="status" class="skeleton line" style="width: 100px;"></div></td>
        <td><span class="badge"><div role="status" class="skeleton line" style="width: 40px;"></div></span></td>
      </tr>
    </tbody>
  </table>
</div>
```

## About role="status"

- Provides accessibility support, telling screen readers this is loading state
- Combined with `aria-live` can notify users content is loading
