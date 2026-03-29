# Accordion

Demo: https://oat.ink/demo/#accordion

Uses native `<details>` + `<summary>`, **no classes needed**.

## Basic Usage

```html
<details>
  <summary>Click to expand</summary>
  <p>Content revealed when expanded.</p>
</details>
```

## Grouped (Mutually Exclusive)

Set the same `name` attribute on multiple `details` elements for radio-like behavior:

```html
<details name="faq">
  <summary>What is Oat UI?</summary>
  <p>Oat UI is a minimal, dependency-free frontend UI library.</p>
</details>

<details name="faq">
  <summary>How do I get started?</summary>
  <p>Simply include the CSS file, no installation required.</p>
</details>

<details name="faq">
  <summary>What browsers are supported?</summary>
  <p>All modern browsers are supported.</p>
</details>
```

## Notes

- The `name` attribute value groups elements; only one can be open at a time within a group
- Content is collapsed by default
- Add the `open` attribute to expand by default
