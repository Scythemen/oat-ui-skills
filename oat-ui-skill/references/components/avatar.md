# Avatar

`<figure data-variant="avatar">` wraps images or abbreviations.

## Image Avatar

```html
<figure data-variant="avatar" aria-label="Jane Doe">
  <img src="/avatar.svg" alt="">
</figure>
```

## Abbreviation Avatar

```html
<figure data-variant="avatar" aria-label="Jane">
  <abbr title="Jane Doe">JD</abbr>
</figure>
```

## Sizes

```html
<!-- Small -->
<figure data-variant="avatar" class="small">...</figure>

<!-- Large -->
<figure data-variant="avatar" class="large">...</figure>
```

## Grouped Avatars (Multiple)

```html
<figure data-variant="avatar" role="group" aria-label="Team members">
  <img src="/a.svg" alt="">
  <img src="/b.svg" alt="">
  <img src="/c.svg" alt="">
</figure>
```

## Complete Example

```html
<!-- Avatar in a user card -->
<article class="card">
  <header style="display: flex; align-items: center; gap: var(--space-2);">
    <figure data-variant="avatar" aria-label="John Smith">
      <img src="/users/john.jpg" alt="">
    </figure>
    <div>
      <h3>John Smith</h3>
      <p style="color: var(--text-muted);">Product Manager</p>
    </div>
  </header>
</article>
```
