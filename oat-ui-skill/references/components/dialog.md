# Dialog

Demo: https://oat.ink/demo/#dialog

Native `<dialog>` element with automatic focus trapping and keyboard support.

## Basic Modal

```html
<dialog id="my-dialog">
  <form method="dialog">
    <header>
      <h3>Dialog Title</h3>
      <p>Dialog description</p>
    </header>
    <div>
      <p>Dialog content area.</p>
    </div>
    <footer>
      <button type="button" commandfor="my-dialog" command="close">Cancel</button>
      <button value="confirm">Confirm</button>
    </footer>
  </form>
</dialog>

<button commandfor="my-dialog" command="show-modal">Open Dialog</button>
```

## Attributes

| Attribute | Value | Description |
|-----------|-------|-------------|
| `commandfor` | dialog ID | Points to the target dialog, e.g., `commandfor="my-dialog"` |
| `command` | `show-modal` | Shows as modal dialog |
| `command` | `close` | Closes the dialog |
| `closedby` | `any` | Clicking outside closes the dialog |
| `method` | `dialog` | Form submission closes dialog and returns value |

## Click Outside to Close

```html
<dialog id="my-dialog" closedby="any">
  <form method="dialog">
    <header><h3>Title</h3></header>
    <div>Click outside to close</div>
    <footer>
      <button type="button" commandfor="my-dialog" command="close">Close</button>
    </footer>
  </form>
</dialog>

<button commandfor="my-dialog" command="show-modal">Open</button>
```

## Getting Return Value

```javascript
const dialog = document.getElementById('my-dialog');
dialog.addEventListener('close', () => {
  console.log('Dialog return value:', dialog.returnValue);
});
```

## Confirm Action Example

```html
<dialog id="confirm-delete">
  <form method="dialog">
    <header>
      <h3>Confirm Delete</h3>
      <p>This action cannot be undone.</p>
    </header>
    <footer>
      <button commandfor="confirm-delete" command="close">Cancel</button>
      <button data-variant="danger" value="delete">Delete</button>
    </footer>
  </form>
</dialog>

<button commandfor="confirm-delete" command="show-modal" data-variant="danger">
  Delete Item
</button>
```

## How It Works

1. `<dialog id="my-dialog">` defines the dialog
2. Trigger button adds `commandfor="my-dialog"` to point to the dialog
3. Trigger button adds `command="show-modal"` to mean "show modal"
4. Close button adds `command="close"` to mean "close"
