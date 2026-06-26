# Maintenance Mode

## Purpose

Display a maintenance message to visitors while allowing administrators to access the website normally.

---

## Code

```php
function wp_maintenance_mode() {
    if (!current_user_can('edit_themes') || !is_user_logged_in()) {
        wp_die('<h1>Website Under Maintenance</h1><p>We will be back shortly.</p>');
    }
}
add_action('get_header', 'wp_maintenance_mode');
```

---

## Where to Add

Add this code to your active theme's `functions.php` file.

---

## Expected Result

- Visitors see a maintenance page.
- Logged-in administrators can still access the website.

---

## Compatibility

- WordPress 5.x+
- WordPress 6.x+

---

## Notes

Use this only for short maintenance periods. For longer maintenance, consider using a dedicated maintenance mode plugin.
