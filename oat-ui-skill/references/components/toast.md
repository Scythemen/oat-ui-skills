# Toast

JS API: `ot.toast(message, title?, options?)`

## Basic Usage

```javascript
ot.toast('Action completed', 'Success', { variant: 'success' });
ot.toast('Error occurred', 'Error', { variant: 'danger', placement: 'top-left' });
ot.toast('Warning message', 'Warning', { variant: 'warning' });
ot.toast('New notification', 'Info');
```

## Options

| Option | Default | Description |
|--------|---------|-------------|
| `variant` | `''` | success/danger/warning |
| `placement` | `'top-right'` | Position |
| `duration` | `4000` | Milliseconds, 0 = persistent |

## Placement Options

```javascript
ot.toast('Message', 'Title', { placement: 'top-right' });    // Top right
ot.toast('Message', 'Title', { placement: 'top-left' });     // Top left
ot.toast('Message', 'Title', { placement: 'bottom-right' }); // Bottom right
ot.toast('Message', 'Title', { placement: 'bottom-left' });  // Bottom left
```

## Persistent Toast

```javascript
ot.toast('Terms of Service', 'Please Read', { variant: '', duration: 0 });
```

## Clear Toast

```javascript
ot.toast.clear();              // Clear all
ot.toast.clear('top-right');   // Clear specific placement
```

## Custom Content

```html
<template id="undo-toast">
  <output class="toast" data-variant="success">
    <h6 class="toast-title">Changes saved</h6>
    <p>Your document has been updated.</p>
    <button class="small" onclick="this.closest('.toast').remove()">OK</button>
  </output>
</template>

<button onclick="ot.toast.el(document.querySelector('#undo-toast'), { duration: 8000 })">
  Show Custom Toast
</button>
```

## Use Cases

- Operation success/failure feedback
- Form validation error messages
- Async operation status notifications
- Undo action prompts

## Notes

- Requires `oat-ui.js` and the `ot` object to be initialized
- Toast automatically disappears after the specified duration
- With `duration: 0`, manual dismissal is required
