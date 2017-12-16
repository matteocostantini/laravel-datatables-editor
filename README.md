# Laravel DataTables Editor Plugin.

[![Laravel 5.5](https://img.shields.io/badge/Laravel-5.5-orange.svg)](http://laravel.com)
[![Latest Stable Version](https://img.shields.io/packagist/v/yajra/laravel-datatables-editor.svg)](https://packagist.org/packages/yajra/laravel-datatables-editor)
[![Build Status](https://travis-ci.org/yajra/laravel-datatables-editor.svg?branch=master)](https://travis-ci.org/yajra/laravel-datatables-editor)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/yajra/laravel-datatables-editor/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/yajra/laravel-datatables-editor/?branch=master)
[![Total Downloads](https://img.shields.io/packagist/dt/yajra/laravel-datatables-editor.svg)](https://packagist.org/packages/yajra/laravel-datatables-editor)
[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://packagist.org/packages/yajra/laravel-datatables-editor)

This package is a plugin of [Laravel DataTables](https://github.com/yajra/laravel-datatables) for processing [DataTables Editor](https://editor.datatables.net/) integration.

> Special thanks to [@bellwood](https://github.com/bellwood) and [@DataTables](https://github.com/datatables) for being [generous](https://github.com/yajra/laravel-datatables/issues/1548) for providing a license to support the development of this package.

## Requirements

- [Laravel 5.5](https://github.com/laravel/framework)
- [Laravel DataTables v8.x](https://github.com/yajra/laravel-datatables)

## Documentations

- COMING SOON!

## Features

- DataTables Editor CRUD actions supported.
- Inline editing.
- Bulk edit & delete function.
- CRUD validation.
- CRUD pre / post events hooks.
- Artisan command for DataTables Editor generation.

## ROAD MAP
- ~~Add artisan command to generate DataTablesEditor stub.~~
- ~~Fix issue with edit action where unmodified column are being added on the request.~~
 
    This only happens when the field is [password](http://luik.datatables.net/forums/discussion/34151/how-do-i-prevent-password-field-from-changing-every-time-a-row-is-edited).
    The solution is to add an empty password on response.
     
    ```php
    datatables(User::query())->setRowId('id')->addColumn('password', '')->toJson()
    ```

- Docs, docs, docs...
- Create demo site.

## Quick Installation

`composer require yajra/laravel-datatables-editor:^1.0`

And that's it! Start building out some awesome DataTables Editor!

## Contributing

Please see [CONTRIBUTING](https://github.com/yajra/laravel-datatables-editor/blob/master/.github/CONTRIBUTING.md) for details.

## Security

If you discover any security related issues, please email [aqangeles@gmail.com](mailto:aqangeles@gmail.com) instead of using the issue tracker.

## Credits

- [Arjay Angeles](https://github.com/yajra)
- [All Contributors](https://github.com/yajra/laravel-datatables-editor/graphs/contributors)

## License

The MIT License (MIT). Please see [License File](https://github.com/yajra/laravel-datatables-editor/blob/master/LICENSE.md) for more information.

## Buy me a coffee

<a href='https://pledgie.com/campaigns/29515'><img alt='Click here to lend your support to: Laravel DataTables and make a donation at pledgie.com !' src='https://pledgie.com/campaigns/29515.png?skin_name=chrome' border='0' ></a>
<a href='https://www.patreon.com/bePatron?u=4521203'><img alt='Become a Patron' src='https://s3.amazonaws.com/patreon_public_assets/toolbox/patreon.png' border='0' width='200px' ></a>
