# Badge

Demo: https://oat.ink/demo/#badge

`<span class="badge">` inline badge for labels and status markers.

## Variants

```html
<span class="badge">Default</span>
<span class="badge secondary">Secondary</span>
<span class="badge outline">Outline</span>
<span class="badge success">Success</span>
<span class="badge warning">Warning</span>
<span class="badge danger">Danger</span>
```

## In Tables

```html
<table>
  <thead>
    <tr><th>Name</th><th>Status</th></tr>
  </thead>
  <tbody>
    <tr>
      <td>Alice</td>
      <td><span class="badge success">Active</span></td>
    </tr>
    <tr>
      <td>Bob</td>
      <td><span class="badge warning">Pending</span></td>
    </tr>
    <tr>
      <td>Charlie</td>
      <td><span class="badge danger">Disabled</span></td>
    </tr>
  </tbody>
</table>
```

## In Buttons

```html
<button>
  Notifications <span class="badge danger">3</span>
</button>
```
