# Card

Add `.card` to any element, commonly used with `<article>`.

## Basic Card

```html
<article class="card">
  <header>
    <h3>Card Title</h3>
    <p>Card description text</p>
  </header>
  <p>Card body content.</p>
  <footer>
    <button class="outline">Cancel</button>
    <button>Confirm</button>
  </footer>
</article>
```

## Header and Footer Layout

Use `.hstack` on footer for horizontal layout:

```html
<article class="card">
  <header>
    <h3>User Info</h3>
    <p>Manage your profile</p>
  </header>
  <div>
    <p>Edit your personal information and settings here.</p>
  </div>
  <footer class="hstack">
    <button class="outline">Cancel</button>
    <button data-variant="primary">Save</button>
  </footer>
</article>
```

## Nested Cards

```html
<div class="row">
  <div class="col-4">
    <article class="card">
      <header><h4>Stats Card</h4></header>
      <p>Content area.</p>
    </article>
  </div>
  <div class="col-4">
    <article class="card">
      <header><h4>Another Card</h4></header>
      <p>More content.</p>
    </article>
  </div>
</div>
```
