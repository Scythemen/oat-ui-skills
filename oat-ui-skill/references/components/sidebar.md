# Sidebar

Layout attribute system supporting sidebar and top navigation.

## Basic Sidebar

```html
<div data-sidebar-layout>
  <aside data-sidebar>
    <nav>
      <ul>
        <li><a href="#" aria-current="page">Home</a></li>
        <li><a href="#">Users</a></li>
        <li>
          <details open>
            <summary>Settings</summary>
            <ul>
              <li><a href="#">General</a></li>
              <li><a href="#">Security</a></li>
            </ul>
          </details>
        </li>
      </ul>
    </nav>
    <footer>
      <button class="outline sm" style="width: 100%;">Logout</button>
    </footer>
  </aside>
  <main>
    <div style="padding: var(--space-3);">
      Main content area
    </div>
  </main>
</div>
```

## With Top Navigation

```html
<body data-sidebar-layout>
  <nav data-topnav>
    <button data-sidebar-toggle class="outline">☰</button>
    <span>App Name</span>
  </nav>
  <aside data-sidebar>
    <nav>
      <ul>
        <li><a href="#" aria-current="page">Home</a></li>
        <li><a href="#">Products</a></li>
        <li><a href="#">About</a></li>
      </ul>
    </nav>
  </aside>
  <main>
    <div style="padding: var(--space-3);">
      <h1>Welcome</h1>
      <p>This is the main content area.</p>
    </div>
  </main>
</body>
```

## Attributes

| Attribute | Purpose |
|-----------|---------|
| `data-sidebar-layout` | Enables sidebar layout |
| `data-sidebar` | Sidebar container |
| `data-topnav` | Top navigation bar |
| `data-sidebar-toggle` | Toggle button (can bind JS) |
| `aria-current="page"` | Marks current page |

## Responsive Sidebar (with JS Toggle)

```html
<body data-sidebar-layout>
  <nav data-topnav>
    <button data-sidebar-toggle class="outline" onclick="toggleSidebar()">☰</button>
    <span>Admin Dashboard</span>
  </nav>
  <aside data-sidebar id="sidebar">
    <nav>
      <ul>
        <li><a href="#" aria-current="page">Dashboard</a></li>
        <li><a href="#">Orders</a></li>
        <li><a href="#">Customers</a></li>
      </ul>
    </nav>
  </aside>
  <main>
    <div style="padding: var(--space-3);">
      Content
    </div>
  </main>
</body>

<script>
  function toggleSidebar() {
    const sidebar = document.getElementById('sidebar');
    sidebar.hasAttribute('hidden') ? sidebar.removeAttribute('hidden') : sidebar.setAttribute('hidden', '');
  }
</script>
```
