# Odnoklassniki OAuth2 client provider

[![Build Status](https://travis-ci.org/rakeev/oauth2-odnoklassniki.svg?branch=master)](https://travis-ci.org/rakeev/oauth2-odnoklassniki)
[![Latest Stable Version](https://poser.pugx.org/aego/oauth2-odnoklassniki/v/stable.svg)](https://packagist.org/packages/aego/oauth2-odnoklassniki)
[![License](https://poser.pugx.org/aego/oauth2-odnoklassniki/license.svg)](https://packagist.org/packages/aego/oauth2-odnoklassniki)

This package provides [Odnoklassniki](http://ok.ru) integration for [OAuth2 Client](https://github.com/thephpleague/oauth2-client) by the League.

## Installation

```sh
composer require aego/oauth2-odnoklassniki
```

## Usage

```php
$provider = new Aego\OAuth2\Client\Provider\Odnoklassniki([
    'clientId'  =>  '1234567890',
    'clientPublic' => 'BA57A2DACCE55C0DE',
    'clientSecret'  =>  '5ADC0DE2ADD1C7ED70C0FFEE',
    'redirectUri' => 'https://example.org/oauth-endpoint',
]);
```

Please pay attention to additional _clientPublic_ parameter — provider requires both numeric and symbolic application IDs.
