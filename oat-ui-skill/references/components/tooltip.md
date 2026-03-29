# Tooltip

Demo: https://oat.ink/demo/#tooltip

The `title` attribute activates Oat UI's default tooltip.

## Basic Usage

```html
<button title="Save your changes">Save</button>
<button title="Delete item" data-variant="danger">Delete</button>
<a href="#" title="View your profile">Profile</a>
```

## Danger Action Tooltip

```html
<button title="This action cannot be undone" data-variant="danger">Delete Account</button>
```

## Image Tooltip

Replaced elements like images need a parent wrapper:

```html
<span title="User avatar"><img src="/avatar.jpg" alt="" height="32"></span>
```

## Icon Button Tooltips

```html
<button class="outline" title="Refresh">
  <svg width="16" height="16" viewBox="0 0 24 24"><path d="M..."/></svg>
</button>

<button class="outline" title="Share">
  <svg width="16" height="16" viewBox="0 0 24 24"><path d="M..."/></svg>
</button>
```

## Toolbar Example

```html
<div class="hstack">
  <button class="outline small" title="Undo">↩</button>
  <button class="outline small" title="Redo">↪</button>
  <button class="outline small" title="Save">💾</button>
  <button class="outline small" title="Print">🖨</button>
</div>
```

## How It Works

Oat UI's Tooltip uses the browser's native `title` attribute. No additional JS or CSS is required — the browser handles the display automatically.

## Notes

- Use semantic `title` text
- Do not include HTML in `title`
- For replaced elements like images, always wrap in `<span>` or another element
