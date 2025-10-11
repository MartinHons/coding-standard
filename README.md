# PHP Coding Standard

A PHP coding standard based on slevomat/coding-standard.

## Installation

Install the package via Composer:

```bash
composer require martinhons/coding-standard --dev
```

## Usage

### Basic Usage

After installation, you can run it directly:

```bash
vendor/bin/phpcs <YOUR_CODE_DIRECTORIES>
vendor/bin/phpcbf <YOUR_CODE_DIRECTORIES>
```

### Recommended Setup

For easier usage, add the following scripts to your `composer.json`:

```json
{
    "scripts": {
        "cs": "phpcs <YOUR_CODE_DIRECTORIES>",
        "csf": "phpcbf <YOUR_CODE_DIRECTORIES>"
    }
}
```

Replace `<YOUR_CODE_DIRECTORIES>` with your actual source directories (e.g. `src tests`).

Then you can run:

```bash
composer cs   # Check coding standards
composer csf  # Fix coding standards automatically
```
