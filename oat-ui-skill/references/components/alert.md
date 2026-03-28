# Alert

`role="alert"` activates styling, `data-variant` selects the type.

## Variants

```html
<!-- Default -->
<div role="alert">Default informational message</div>

<!-- Success -->
<div role="alert" data-variant="success"><strong>Success!</strong> Your changes have been saved.</div>

<!-- Warning -->
<div role="alert" data-variant="warning"><strong>Warning!</strong> Please check your input.</div>

<!-- Error -->
<div role="alert" data-variant="error"><strong>Error!</strong> Something went wrong, please try again.</div>
```

## data-variant Values

| Value | Purpose | Color |
|-------|---------|-------|
| `success` | Success message | Green |
| `warning` | Warning message | Yellow |
| `error` | Error message | Red |
| default | General message | Gray |

## Use Cases

- Form submission feedback
- Global page notifications
- Operation status messages
