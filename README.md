# Laravel JWT API 

<a href="https://github.com/avinmaster/laravel-jwt-api/actions"><img src="https://github.com/avinmaster/laravel-jwt-api/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/avinmaster/laravel-jwt-api"><img src="https://poser.pugx.org/avinmaster/laravel-jwt-api/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/avinmaster/laravel-jwt-api"><img src="https://poser.pugx.org/avinmaster/laravel-jwt-api/v/stable.svg" alt="Latest Stable Version"></a>

> A Laravel JWT API starter kit.

## Features

- Laravel 8
- Login, register, email verification and password reset
- Authentication with JWT
- Socialite integration

## Installation

- `composer create-project --prefer-dist avinmaster/laravel-jwt-api`
- Edit `.env` and set your database connection details
- (When installed via git clone or download, run `php artisan key:generate` and `php artisan jwt:secret`)
- `php artisan migrate`
- `npm install`

## Usage

### Socialite

This project comes with GitHub as an example for [Laravel Socialite](https://laravel.com/docs/5.8/socialite).

To enable the provider create a new GitHub application and use `https://example.com/api/oauth/github/callback` as the Authorization callback URL.

Edit `.env` and set `GITHUB_CLIENT_ID` and `GITHUB_CLIENT_SECRET` with the keys form your GitHub application.

For other providers you may need to set the appropriate keys in `config/services.php` and redirect url in `OAuthController.php`.
<hr />

### Email Verification

To enable email verification make sure that your `App\User` model implements the `Illuminate\Contracts\Auth\MustVerifyEmail` contract.
<hr />

# Testing

### Run all unit and feature tests
```bash
vendor/bin/phpunit
```

## Changelog

Please see [CHANGELOG](https://github.com/avinmaster/laravel-jwt-api/CHANGELOG.md) for more information what has changed recently.
