# Remove WordPress Version

## Purpose

Hide the WordPress version number from your website to improve security.

---

## Code

```php
// Remove WordPress version number
remove_action('wp_head', 'wp_generator');
```

---

## Where to Add

Add this code to your active theme's `functions.php` file or use a code snippets plugin.

---

## Expected Result

- WordPress version is no longer displayed in the page source.
- Makes it slightly harder for automated bots to identify your WordPress version.

---

## Compatibility

- WordPress 5.x+
- WordPress 6.x+

---

## Notes

This is a small security improvement. It should be combined with other security best practices such as disabling XML-RPC (if not needed), limiting login attempts, and keeping WordPress, themes, and plugins up to date.
