# Upgrade Guide

- [Upgrade To 2.2.1](#upgrade-2.2.1)
- [Upgrade To 2.2](#upgrade-2.2)
- [Upgrade To 2.1](#upgrade-2.1)
- [Upgrade To 2.0.1](#upgrade-2.0.1)
- [Upgrade To 2.0](#upgrade-2.0)
- [Upgrading To 1.1](#upgrade-1.1)

<a name="upgrade-2.2.1"></a>
## Upgrade from 2.2 to 2.2.1

- Replace 2 files `core/base/resources/views/layouts/master.blade.php` & `core/table/src/Abstracts/TableAbstract.php`

<a name="upgrade-2.2"></a>
## Upgrade from 2.1 to 2.2

- Override folder /core & /plugins with new source code.
- Run `php artisan vendor:publish --tag=public --force`
- Run `php artisan vendor:publish --tag=lang --force`
- Run `composer install` to update vendor packages.
- Run `php artisan migrate` to update database.

<a name="upgrade-2.1"></a>
## Upgrade from 2.0.1 to 2.1

- Run `composer install` to update vendor packages.
- Run `php artisan migrate` to update database.
- Deprecated classes: Botble\Base\Tables\TableAbstract & Botble\Base\Tables\TableBuilder will be removed in the next version, 
please change to use Botble\Table\Abstracts\TableAbstract & Botble\Table\TableBuilder

<a name="upgrade-2.0.1"></a>
## Upgrade from 2.0 to 2.0.1

- Override folder /core and /plugins
- Run "php artisan vendor:publish --tag=public --force" to update assets.
- Run "php artisan migrate" to update database.

<a name="upgrade-2.0"></a>
## Upgrade from 1.1 to 2.0

- Copy your theme to new source code.
- Run `composer install` to update vendor packages.
- Run `php artisan migrate` to update database.

> {warning} Old custom plugins which you built with v1.1 will not work on v2.0.

<a name="upgrade-1.1"></a>
## Upgrade from 1.0 to 1.1
- Using new source code from Codecanyon.
- Run `composer install` to update vendor packages.
- Run `php artisan migrate` to update database.