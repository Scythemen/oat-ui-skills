---
name: oat-ui-skill
description: Oat UI ultra-lightweight UI library assistant. Use this skill when users want to create buttons, forms, dialogs, menus, badges, cards, grids, or any other UI components with Oat UI. Covers all Oat UI components with HTML usage, attributes, class names, and code examples. Also covers CSS utilities for layout, spacing, alignment (`.hstack`, `.vstack`, `.gap-*`, `.justify-*`, `.mt-*`, etc.).
---

# Oat UI Skill

Oat UI is an ultra-lightweight, dependency-free frontend UI library. **HTML-first** — use semantic HTML tags directly with minimal or no class names for beautiful interfaces.

## Installation

### CDN (Recommended)

```html
<head>
  <link rel="stylesheet" href="https://unpkg.com/@knadh/oat/oat.min.css">
</head>
<body>
  <!-- Page content -->

  <script src="https://unpkg.com/@knadh/oat/oat.min.js" defer></script>
</body>
```

### npm

```bash
npm install @knadh/oat
```

Then import in your project:
```javascript
import '@knadh/oat';          // JS (required for Web Components)
import '@knadh/oat/oat.css';  // CSS
```

### Download

Direct download pre-built files:
- CSS: https://unpkg.com/@knadh/oat/oat.min.css
- JS: https://unpkg.com/@knadh/oat/oat.min.js

**Note:** JS is only required when using Web Components like Dialog, Dropdown, Tabs.

## Components Quick Reference

| Component | Usage | Key Attributes/Classes |
|-----------|-------|------------------------|
| [Typography](references/components/typography.md) | Semantic HTML | No classes needed |
| [Accordion](references/components/accordion.md) | `<details>` + `<summary>` | `name` for grouping |
| [Alert](references/components/alert.md) | `role="alert"` | `data-variant` |
| [Avatar](references/components/avatar.md) | `<figure data-variant="avatar">` | `.small` / `.large` |
| [Badge](references/components/badge.md) | `.badge` | `secondary`, `outline`, `success`, `warning`, `danger` |
| [Breadcrumb](references/components/breadcrumb.md) | `<nav>` + `<ol>` | `.unstyled`, `.hstack` |
| [Button](references/components/button.md) | `<button>` / `<a class="button">` | `data-variant`, `outline`, `ghost`, `small`, `large` |
| [Card](references/components/card.md) | `.card` | `.hstack` |
| [Dialog](references/components/dialog.md) | `<dialog>` | `commandfor`, `command="show-modal"`, `closedby` |
| [Dropdown](references/components/dropdown.md) | `<ot-dropdown>` | `popovertarget`, `popover` |
| [Form](references/components/form.md) | `<label>` wrapping | `data-field` is optional CSS style |
| [Grid](references/components/grid.md) | `.container` + `.row` + `.col-{n}` | 12-column system |
| [Meter](references/components/meter.md) | `<meter>` | `value`, `low`, `high`, `optimum` |
| [Pagination](references/components/pagination.md) | Button + `<nav>` | `aria-current="page"` |
| [Progress](references/components/progress.md) | `<progress>` | `value`, `max` |
| [Sidebar](references/components/sidebar.md) | `data-sidebar-layout` | `data-sidebar`, `data-topnav`, `data-sidebar-toggle` |
| [Skeleton](references/components/skeleton.md) | `.skeleton` + `role="status"` | `.line`, `.box` |
| [Spinner](references/components/spinner.md) | `aria-busy="true"` | `data-spinner` |
| [Switch](references/components/switch.md) | `<input type="checkbox" role="switch">` | `checked`, `disabled` |
| [Table](references/components/table.md) | `<table>` + `.table` | Responsive scrolling |
| [Tabs](references/components/tabs.md) | `<ot-tabs>` | `role="tablist"`, `role="tab"`, `role="tabpanel"` |
| [Toast](references/components/toast.md) | JS API | `ot.toast(message, title, options)` |
| [Tooltip](references/components/tooltip.md) | `title` attribute | — |
| [Utilities](references/utilities.md) | CSS utility classes | `.hstack`, `.vstack`, `.gap-*`, `.justify-*`, `.mt-*`, `.mb-*`, `.flex`, `.text-light`, `.w-100` |

## Common Classes

| Class | Purpose |
|-------|---------|
| `.hstack` | Horizontal stack (flex row, centered, gap) |
| `.vstack` | Vertical stack (flex column, gap) |
| `.flex` | Display flex |
| `.flex-col` | Flex column direction |
| `.items-center` | Align items center |
| `.justify-center` | Justify content center |
| `.justify-between` | Justify content space-between |
| `.justify-end` | Justify content flex-end |
| `.gap-1` / `.gap-2` / `.gap-4` | Explicit gap overrides |
| `.mt-2` / `.mt-4` / `.mt-6` | Margin block start |
| `.mb-2` / `.mb-4` / `.mb-6` | Margin block end |
| `.p-4` | Padding |
| `.w-100` | Full width |
| `.align-left` / `.align-center` / `.align-right` | Text alignment |
| `.text-light` / `.text-lighter` | Muted / faint text color |
| `.unstyled` | Remove default list/link styles |
| `.outline` | Outline button style |
| `.small` / `.sm` | Small size |
| `.large` | Large size |

See [utilities.md](references/utilities.md) for full examples.

## Usage

When user needs to create any UI component or layout:
1. Identify the most suitable Oat UI component for the user's needs
2. Read the corresponding component file for detailed usage
3. Check [utilities.md](references/utilities.md) for layout/spacing/alignment needs
4. Output complete HTML code examples
5. If JS is needed (e.g., Toast), provide the JavaScript code

**Project:** https://oat.ink/ | **GitHub:** https://github.com/knadh/oat
