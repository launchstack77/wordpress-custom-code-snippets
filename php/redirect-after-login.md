# Redirect Users After Login

## Purpose

Redirect users to a specific page after successful login.

---

## Code

```php
function custom_login_redirect($redirect_to, $request, $user) {

    return home_url('/dashboard/');

}

add_filter('login_redirect', 'custom_login_redirect', 10, 3);
```

---

## Where to Add

Add this code to your active theme's `functions.php` file or a Code Snippets plugin.

---

## Expected Result

Users are redirected to `/dashboard/` after logging in.

---

## Compatibility

- WordPress 5.x+
- WordPress 6.x+

---

## Notes

Replace `/dashboard/` with any page slug you want users to visit after login.
