# 📧 Email Value Object (PHP)

This repository contains a simple, immutable **Email value object** in PHP. It encapsulates an email address and enforces strict validation on creation. This design is commonly used in **domain-driven design (DDD)** to represent concepts with guaranteed validity.

## ✨ Features

- ✅ Enforces strict validation using `FILTER_VALIDATE_EMAIL`
- 🚫 Throws an `InvalidArgumentException` for invalid input
- 📦 Immutable value object pattern
- 🔒 Type-safe via `declare(strict_types=1)`
- 🧪 Unit-testable (compatible with PHPUnit)

## 🧩 Example Usage

```php
<?php

require 'src/Email.php';

$email = Email::fromString('user@example.com');
echo $email; // Outputs: user@example.com
