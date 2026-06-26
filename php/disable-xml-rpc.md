# Disable XML-RPC

## Purpose

Disable XML-RPC to improve security.

## Code

```php
add_filter('xmlrpc_enabled', '__return_false');
```

## Where to Add

functions.php

## Expected Result

XML-RPC requests will be disabled.
```
