# Meter

Native `<meter>` element with automatic color based on value.

## Basic Usage

```html
<meter value="0.8" min="0" max="1" low="0.3" high="0.7" optimum="1"></meter>
```

## Color States

```html
<!-- High (green) - value above high and close to optimum -->
<meter value="0.9" min="0" max="1" low="0.3" high="0.7" optimum="1"></meter>

<!-- Medium (yellow) - value between low and high -->
<meter value="0.5" min="0" max="1" low="0.3" high="0.7" optimum="1"></meter>

<!-- Low (red) - value below low -->
<meter value="0.2" min="0" max="1" low="0.3" high="0.7" optimum="1"></meter>
```

## Attributes

| Attribute | Description |
|-----------|-------------|
| `value` | Current value |
| `min` | Minimum (default 0) |
| `max` | Maximum (default 1) |
| `low` | Low threshold |
| `high` | High threshold |
| `optimum` | Optimal value |

## Use Cases

- File upload progress
- Disk usage
- Battery level
- Metric dashboards

```html
<label>
  Battery Level
  <meter value="0.75" min="0" max="1" low="0.2" high="0.8" optimum="1"></meter>
</label>
```
