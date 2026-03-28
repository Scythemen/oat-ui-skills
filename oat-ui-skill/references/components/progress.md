# Progress

Native `<progress>` element.

## Basic Usage

```html
<progress value="60" max="100"></progress>
```

## With Percentage

```html
<label>
  Upload Progress
  <progress value="30" max="100"></progress>
  <span data-hint>30%</span>
</label>
```

## Dynamic Progress Bar

```html
<label for="upload-progress">File Upload</label>
<progress id="upload-progress" value="0" max="100"></progress>
<span data-hint id="progress-text">0%</span>

<script>
  const progress = document.getElementById('upload-progress');
  const text = document.getElementById('progress-text');
  // Simulate upload
  let value = 0;
  const interval = setInterval(() => {
    value += 10;
    progress.value = value;
    text.textContent = value + '%';
    if (value >= 100) clearInterval(interval);
  }, 500);
</script>
```

## Attributes

| Attribute | Description |
|-----------|-------------|
| `value` | Current progress value |
| `max` | Maximum value (default 1) |

## Use Cases

- File upload progress
- Operation completion
- Loading state indicator
