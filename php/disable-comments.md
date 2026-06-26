# Disable Comments in WordPress

## Purpose

Completely disables comments on a WordPress website.

## Add this code to functions.php

```php
function disable_comments_post_types_support() {
    $post_types = get_post_types();

    foreach ($post_types as $post_type) {
        if(post_type_supports($post_type, 'comments')) {
            remove_post_type_support($post_type, 'comments');
            remove_post_type_support($post_type, 'trackbacks');
        }
    }
}
add_action('admin_init', 'disable_comments_post_types_support');
```

## Use Case

Useful for business websites that do not require comments.
