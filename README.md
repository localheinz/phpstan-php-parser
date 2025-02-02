# PHP-Parser extension for PHPStan

[![Build Status](https://travis-ci.org/phpstan/phpstan-php-parser.svg)](https://travis-ci.org/phpstan/phpstan-php-parser)
[![Latest Stable Version](https://poser.pugx.org/phpstan/phpstan-php-parser/v/stable)](https://packagist.org/packages/phpstan/phpstan-php-parser)
[![License](https://poser.pugx.org/phpstan/phpstan-php-parser/license)](https://packagist.org/packages/phpstan/phpstan-php-parser)

* [PHPStan](https://github.com/phpstan/phpstan)
* [PHP-Parser](https://github.com/nikic/php-parser)

This extension provides the following feature:

* If you register `PhpParser\NodeVisitor\NameResolver` visitor on `PhpParser\NodeTraverser`, new `$namespacedName` property becomes available on nodes that already have a `$name` property. This extension defines that property.

## Installation

To use this extension, require it in [Composer](https://getcomposer.org/):

```
composer require --dev phpstan/phpstan-php-parser
```

If you also install [phpstan/extension-installer](https://github.com/phpstan/extension-installer) then you're all set!

<details>
  <summary>Manual installation</summary>

If you don't want to use `phpstan/extension-installer`, include extension.neon in your project's PHPStan config:

```
includes:
    - vendor/phpstan/phpstan-php-parser/extension.neon
```
</details>
