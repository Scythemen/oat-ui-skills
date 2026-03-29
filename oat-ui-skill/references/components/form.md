# Form Elements

Demo: https://oat.ink/demo/#form

**About `data-field`:** This is an optional CSS margin style attribute that controls element spacing. **It is not a functional requirement** and can be added or omitted freely.

## Basic Inputs

```html
<label>
  Name
  <input type="text" placeholder="Enter name">
</label>

<label>
  Email
  <input type="email" placeholder="you@example.com">
</label>

<label>
  Password
  <input type="password" placeholder="Password">
</label>
```

## Select

```html
<label>
  Select an option
  <select aria-label="Select an option">
    <option value="">Choose...</option>
    <option value="a">Option A</option>
    <option value="b">Option B</option>
  </select>
</label>
```

## Checkbox and Radio

```html
<label>
  <input type="checkbox"> I agree to the terms
</label>

<fieldset class="hstack">
  <legend>Preference</legend>
  <label><input type="radio" name="pref"> Option A</label>
  <label><input type="radio" name="pref"> Option B</label>
</fieldset>
```

## Input Groups

```html
<fieldset class="group">
  <legend>https://</legend>
  <input type="url" placeholder="subdomain">
  <select aria-label="Select subdomain">
    <option>.example.com</option>
    <option>.org</option>
  </select>
  <button>Go</button>
</fieldset>
```

## Complete Form Example

```html
<form>
  <label>
    Username
    <input type="text" placeholder="Enter username">
  </label>

  <label>
    Email
    <input type="email" placeholder="you@example.com">
  </label>

  <label>
    Password
    <input type="password" placeholder="At least 8 characters">
  </label>

  <label>
    Role
    <select aria-label="Select role">
      <option value="">Choose...</option>
      <option value="admin">Administrator</option>
      <option value="user">Regular User</option>
    </select>
  </label>

  <label>
    Bio
    <textarea rows="4" placeholder="Tell us about yourself"></textarea>
  </label>

  <label>
    <input type="checkbox"> Subscribe to updates
  </label>

  <footer class="hstack">
    <button class="outline">Cancel</button>
    <button data-variant="primary">Register</button>
  </footer>
</form>
```

## Supported Input Types

| Type | Description |
|------|-------------|
| text | Text input |
| email | Email input |
| password | Password input |
| url | URL input |
| datetime-local | Date and time |
| date | Date |
| file | File upload |
| checkbox | Checkbox |
| radio | Radio button |
| range | Range slider |
| textarea | Multi-line text |
| select | Dropdown select |
