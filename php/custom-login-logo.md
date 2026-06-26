# Custom WordPress Login Logo

## Purpose

Replace the default WordPress logo on the login page with your own logo.

---

## Code

```php
function custom_login_logo() {
?>
<style type="text/css">
#login h1 a {
    background-image: url('https://yourdomain.com/logo.png');
    background-size: contain;
    width: 250px;
}
</style>
<?php
}
add_action('login_enqueue_scripts', 'custom_login_logo');
```

---

## Where to Add

Add this code to your active theme's `functions.php` file.

---

## Expected Result

- Displays your custom logo on the WordPress login page.
- Gives clients a branded login experience.

---

## Compatibility

- WordPress 5.x+
- WordPress 6.x+

---

## Notes

Replace `https://yourdomain.com/logo.png` with the URL of your own logo.
