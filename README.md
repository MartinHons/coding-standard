# PHP Coding Standard

A PHP coding standard based on **slevomat/coding-standard**.

## Installation

```bash
composer require martinhons/coding-standard --dev
```

## Basic Usage

For check the coding standard for the `src` and `tests` directories run:
```bash
vendor/bin/phpcs src tests
```

To automatically fix coding standard issues int the `src` and `tests` directories run:
```bash
vendor/bin/phpcbf src tests
```

## Recommended Setup

For easier usage you can add the following scripts to your `composer.json`:

```json
{
    "scripts": {
        "cs": "phpcs --standard=HonsStandard <YOUR_CODE_DIRECTORIES>",
        "csf": "phpcbf --standard=HonsStandard <YOUR_CODE_DIRECTORIES>"
    }
}
```

Replace `<YOUR_CODE_DIRECTORIES>` with your code directory or directories.

Then you can run:

```bash
composer cs   # Check coding standards
composer csf  # Fix coding standards automatically
```
