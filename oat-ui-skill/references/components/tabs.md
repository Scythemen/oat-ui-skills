# Tabs

Demo: https://oat.ink/demo/#tabs

`<ot-tabs>` Web Component. Button count must match panel count.

## Basic Usage

```html
<ot-tabs>
  <div role="tablist">
    <button role="tab">Account</button>
    <button role="tab">Password</button>
    <button role="tab">Notifications</button>
  </div>
  <div role="tabpanel">
    <h3>Account Settings</h3>
    <p>Manage your account information.</p>
  </div>
  <div role="tabpanel">
    <h3>Password Settings</h3>
    <p>Change your password.</p>
  </div>
  <div role="tabpanel">
    <h3>Notification Settings</h3>
    <p>Configure notification preferences.</p>
  </div>
</ot-tabs>
```

## Attributes

| Attribute | Element | Description |
|-----------|---------|-------------|
| `role="tablist"` | Container div | Tab list container |
| `role="tab"` | button | Individual tab |
| `role="tabpanel"` | div | Tab content panel |

## Notes

- **Button count must exactly match panel count**
- Buttons correspond to panels by order
- Requires `<script src="oat-ui.js">`

## Complete Settings Page Example

```html
<ot-tabs>
  <div role="tablist">
    <button role="tab">Profile</button>
    <button role="tab">Security</button>
    <button role="tab">Preferences</button>
  </div>
  <div role="tabpanel">
    <h3>Profile</h3>
    <label>
      Name
      <input type="text" id="name" value="John">
    </label>
    <label>
      Bio
      <textarea id="bio" rows="3">Product Manager</textarea>
    </label>
    <button data-variant="primary">Save</button>
  </div>
  <div role="tabpanel">
    <h3>Security</h3>
    <label>
      New Password
      <input type="password" id="password">
    </label>
    <label>
      Confirm Password
      <input type="password" id="confirm">
    </label>
    <button data-variant="primary">Change Password</button>
  </div>
  <div role="tabpanel">
    <h3>Preferences</h3>
    <label>
      <input type="checkbox" role="switch" checked> Dark Mode
    </label>
  </div>
</ot-tabs>
```
