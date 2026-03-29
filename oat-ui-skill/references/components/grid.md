# Grid

Demo: https://oat.ink/demo/#grid

12-column grid system.

## Basic Structure

```html
<div class="container">
  <div class="row">
    <div class="col-4">col-4</div>
    <div class="col-4">col-4</div>
    <div class="col-4">col-4</div>
  </div>
</div>
```

## Column Offsets

```html
<div class="container">
  <div class="row">
    <div class="col-4 offset-2">col-4 offset-2</div>
    <div class="col-4">col-4</div>
  </div>
</div>
```

## Right Alignment

```html
<div class="container">
  <div class="row">
    <div class="col-4 col-end">col-4 col-end</div>
  </div>
</div>
```

## Responsive Example

```html
<div class="container">
  <div class="row">
    <div class="col-12 col-md-6 col-lg-4">
      <article class="card">
        <header><h4>Card One</h4></header>
        <p>Content</p>
      </article>
    </div>
    <div class="col-12 col-md-6 col-lg-4">
      <article class="card">
        <header><h4>Card Two</h4></header>
        <p>Content</p>
      </article>
    </div>
    <div class="col-12 col-md-12 col-lg-4">
      <article class="card">
        <header><h4>Card Three</h4></header>
        <p>Content</p>
      </article>
    </div>
  </div>
</div>
```

## Class Reference

| Class | Description |
|-------|-------------|
| `.container` | Container |
| `.row` | Row |
| `.col-{n}` | Span n columns (1-12) |
| `.offset-{n}` | Offset by n columns |
| `.col-end` | Align to end |
