# Laravel Quick Deploy Tips and Tricks

Replace `<Name>` with your model name
<hr/>
- ## Edit `.env` file

- ## Reset Migration
```
	php artisan migrate:reset
```

- ## Create a Migration File
```
	php artisan make:migration create_<Name>_table --create=<Name>
```
Edit the migration table @ `database/migrations/create_<Name>_table.php`

- ## Migrate Table
```
	php artisan migrate
```
Double check table for mistakes

- ## Make a Model and a Controller
```
	php artisan make:model <Name> -m
  php artisan make:controller <Name>Controller
```

Check the Model @ `app/<Name>.php`.

Create the Views.

Create `master.blade.php` template on `views` folder and ?Navbar?.

Configure the newly created Controller.

Map the application @ `routes.php`.

- ## ? HTTP Requests
```
	php artisan make:request <Name>FormRequest
```
