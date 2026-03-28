# Dropdown

`<ot-dropdown>` Web Component using native Popover API.

## Menu Dropdown

```html
<ot-dropdown>
  <button popovertarget="demo-menu" class="outline">
    Options <svg width="16" height="16" viewBox="0 0 24 24"><path d="m6 9 6 6 6-6"/></svg>
  </button>
  <menu popover id="demo-menu">
    <button role="menuitem">Profile</button>
    <button role="menuitem">Settings</button>
    <button role="menuitem">Help</button>
    <hr>
    <button role="menuitem">Logout</button>
  </menu>
</ot-dropdown>
```

## Confirm Popup

```html
<ot-dropdown>
  <button popovertarget="demo-confirm" class="outline">Confirm Action</button>
  <article class="card" popover id="demo-confirm">
    <header>
      <h4>Are you sure?</h4>
      <p>This action cannot be undone.</p>
    </header>
    <footer>
      <button class="outline small" popovertarget="demo-confirm">Cancel</button>
      <button data-variant="danger" class="small" popovertarget="demo-confirm">Confirm Delete</button>
    </footer>
  </article>
</ot-dropdown>
```

## Menu Grouping

```html
<ot-dropdown>
  <button popovertarget="file-menu" class="outline">
    File <svg width="12" height="12" viewBox="0 0 24 24"><path d="m6 9 6 6 6-6"/></svg>
  </button>
  <menu popover id="file-menu">
    <button role="menuitem">New</button>
    <button role="menuitem">Open</button>
    <button role="menuitem">Save</button>
    <hr>
    <button role="menuitem">Export</button>
    <button role="menuitem">Print</button>
  </menu>
</ot-dropdown>
```

## Notes

- Requires `<script src="oat-ui.js">` to register the Web Component
- `popovertarget` points to the menu's `id`
- `menu` tag provides native menu semantics
