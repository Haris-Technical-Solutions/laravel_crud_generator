




This Laravel Generator package provides and generate Controller, Model (with eloquent relations) and Views in **Bootstrap** for your development of your applications with single command.

- Will create **Model** with Eloquent relations
- Will create **Controller** with all resources
- Will create **views** in Bootstrap

## Requirements
    Laravel >= 5.5
    PHP >= 7.1

## Installation
1 - Install
```
composer require hts/crud-generator --dev
```
2- Publish the default package's config
```
php artisan vendor:publish --tag=crud
```

## Usage
```
php artisan make:crud {table_name}

php artisan make:crud banks
```

Add a route in `web.php`
```
Route::resource('banks', 'BankController');
```
Route name in plural slug case.

#### Options
 - Custom Route
```
php artisan make:crud {table_name} --route={route_name}
```

## Example

*Model*
![Model](https://i.imgur.com/zTSoYvJ.png)


*Controller*
![Controller](https://i.imgur.com/G1ytmcL.png)


*Listing*
![Listing](https://i.imgur.com/UH5XGuw.png)


*Form*
![Form](https://i.imgur.com/poRiZRO.png)


## Author

M Haris // [Email Me](mailto:pk.harissultani@gmail.com)
