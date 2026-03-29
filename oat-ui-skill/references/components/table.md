# Table

Demo: https://oat.ink/demo/#table

Semantic `<table>` with `.table` container for responsive horizontal scrolling on mobile.

## Basic Table

```html
<div class="table">
  <table>
    <thead>
      <tr><th>Name</th><th>Email</th><th>Role</th><th>Status</th></tr>
    </thead>
    <tbody>
      <tr>
        <td>Alice</td>
        <td>alice@example.com</td>
        <td>Admin</td>
        <td><span class="badge success">Active</span></td>
      </tr>
      <tr>
        <td>Bob</td>
        <td>bob@example.com</td>
        <td>Editor</td>
        <td><span class="badge warning">Pending</span></td>
      </tr>
      <tr>
        <td>Charlie</td>
        <td>charlie@example.com</td>
        <td>User</td>
        <td><span class="badge danger">Disabled</span></td>
      </tr>
    </tbody>
  </table>
</div>
```

## With Sorting

```html
<div class="table">
  <table>
    <thead>
      <tr>
        <th><button class="unstyled">Name ↕</button></th>
        <th><button class="unstyled">Email ↕</button></th>
        <th><button class="unstyled">Role ↕</button></th>
        <th>Status</th>
      </tr>
    </thead>
    <tbody>
      <!-- Data rows -->
    </tbody>
  </table>
</div>
```

## Complete User List

```html
<div class="table">
  <table>
    <thead>
      <tr>
        <th>User</th>
        <th>Email</th>
        <th>Role</th>
        <th>Status</th>
        <th>Actions</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>
          <div style="display: flex; align-items: center; gap: var(--space-2);">
            <figure data-variant="avatar" class="small">
              <img src="/users/1.jpg" alt="">
            </figure>
            <span>Alice</span>
          </div>
        </td>
        <td>alice@example.com</td>
        <td><span class="badge secondary">Admin</span></td>
        <td><span class="badge success">Active</span></td>
        <td>
          <menu class="buttons" style="display: inline-flex;">
            <li><button class="outline small">Edit</button></li>
            <li><button class="outline small" data-variant="danger">Delete</button></li>
          </menu>
        </td>
      </tr>
    </tbody>
  </table>
</div>
```

## Responsive Behavior

The `.table` container automatically adds horizontal scrolling on small screens, ensuring the table doesn't compress or break layout.
