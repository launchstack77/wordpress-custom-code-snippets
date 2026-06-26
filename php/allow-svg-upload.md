# Allow SVG Uploads

## Purpose

Enable SVG file uploads in the WordPress Media Library.

---

## Code

```php
function allow_svg_upload($mimes) {
    $mimes['svg'] = 'image/svg+xml';
    return $mimes;
}

add_filter('upload_mimes', 'allow_svg_upload');
```

---

## Where to Add

Add this code to your active theme's `functions.php` file or a Code Snippets plugin.

---

## Expected Result

- SVG files can be uploaded through the Media Library.

---

## Compatibility

- WordPress 5.x+
- WordPress 6.x+

---

## Notes

SVG files can contain malicious code. Only upload SVGs from trusted sources or use an SVG sanitization plugin.
