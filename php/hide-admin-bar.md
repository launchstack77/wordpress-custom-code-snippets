# Hide Admin Bar

## Purpose

Hide the WordPress admin bar for all users except administrators.

## Code

```php
add_filter('show_admin_bar', '__return_false');
```

## Where to Add

functions.php or Code Snippets plugin.

## Expected Result

The admin toolbar will no longer appear on the frontend.
```
