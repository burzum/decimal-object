#  Decimal Value Object

[![License](https://poser.pugx.org/spryker/decimal/license)](https://packagist.org/packages/spryker/decimal)
[![Minimum PHP Version](https://img.shields.io/badge/php-%3E%3D%207.1-8892BF.svg)](https://php.net/)

Decimal value object for PHP.

## Background
When working with monetary values, normal data types like int or float are not suitable for exact arithmetic.
Handling them as string is a workaround, but as value object you can more easily encapsulate some of the logic. 

### Alternatives
Solutions like https://php-decimal.io require a PHP extension (would make it faster, but also more difficult for some
servers to be available). For details see [wiki](https://github.com/spryker/decimal/wiki).

## Features

- Basic math operations and checks supported
- Immutability
- Handle very large and very small numbers

Note: This library is a sandbox/showcase and for testing right now only.
Alpha-version. Use with Caution.

## Installation

### Requirements

- `bcmath` PHP extension enabled

### Composer (preferred)
```
composer require spryker/decimal:dev-master
```

## Usage

See [Documentation](/docs) for more details.

### Implementations
The following libraries are using the `Decimal` value object:

- [dereuromark/cakephp-decimal](https://github.com/dereuromark/cakephp-decimal) as decimal type replacement for CakePHP ORM.


## TODO
- Rounding
- ceil()/floor() ?
- Assert/check edge case values (very small values)
- sum(), average(), max(), min() as static methods ?
- modulo()/power() ?
- shift() ?
- API naming `add() => plus()`, `subtract() => minus()`, `multiply() => multipliedBy()`, `divide() => devidedBy()` ?
