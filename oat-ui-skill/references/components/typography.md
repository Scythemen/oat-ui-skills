# Typography

Demo: https://oat.ink/demo/#typography

**No classes needed.** Simply use semantic tags and they are styled automatically.

## Tag Reference

| Tag | Purpose |
|-----|---------|
| `<h1>` ~ `<h6>` | Headings |
| `<p>` | Paragraphs (can use `<strong>`, `<em>`, `<a>`) |
| `<code>` | Inline code |
| `<pre><code>` | Code block |
| `<blockquote>` | Block quote |
| `<hr>` | Horizontal rule |
| `<ul>` / `<ol>` | Lists |

## Examples

```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>

<p>This is paragraph text with <strong>bold</strong> and <em>italic</em> styling.</p>

<p><a href="#">Link text</a></p>

<pre><code>const oat = require('oat-ui');
console.log('Code block');</code></pre>

<blockquote>
  <p>This is a block quote.</p>
</blockquote>

<ul>
  <li>List item one</li>
  <li>List item two</li>
</ul>

<hr>
```
