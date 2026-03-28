# Switch

`<input type="checkbox" role="switch">` toggle component.

## Basic Usage

```html
<label>
  <input type="checkbox" role="switch"> Enable notifications
</label>
```

## States

```html
<!-- Default unchecked -->
<input type="checkbox" role="switch">

<!-- Checked -->
<input type="checkbox" role="switch" checked>

<!-- Disabled -->
<input type="checkbox" role="switch" disabled>

<!-- Disabled and checked -->
<input type="checkbox" role="switch" checked disabled>
```

## Complete Example

```html
<div>
  <label>Notification Settings</label>
  <div style="display: flex; flex-direction: column; gap: var(--space-2);">
    <label style="display: flex; justify-content: space-between; align-items: center;">
      <span>Email Notifications</span>
      <input type="checkbox" role="switch" id="notifications" checked>
    </label>
    <label style="display: flex; justify-content: space-between; align-items: center;">
      <span>SMS Notifications</span>
      <input type="checkbox" role="switch">
    </label>
    <label style="display: flex; justify-content: space-between; align-items: center;">
      <span>Push Notifications</span>
      <input type="checkbox" role="switch" checked disabled>
    </label>
  </div>
</div>
```

## Getting Value

```javascript
const switchEl = document.querySelector('input[type="checkbox"][role="switch"]');
switchEl.addEventListener('change', (e) => {
  console.log('Switch state:', e.target.checked);
});
```

## Styling Notes

- Switch is essentially a checkbox, but `role="switch"` gives it specialized styling
- Checked shows as blue track
- Unchecked shows as gray track
- Disabled reduces opacity
