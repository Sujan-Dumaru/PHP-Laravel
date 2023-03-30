# PHP-Laravel

<details>

<summary>Laravel Initial Project Setup</summary>

#### installing laravel globally
````composer global require laravel/installer````


##### create laravel project
````laravel new projectName````


#### run project
````php artisan serve````
</details>

<details>

<summary>Component</summary>

#### Creating Component
```php artisan make:component <ComponentName>```

The command "php artisan make:component modal" is used in Laravel to generate a new component class for a modal. 
This command creates a new PHP class file in the "app/View/Components" directory of your Laravel application.

The generated class file extends the base "Component" class and defines a "render" method 
that returns the HTML markup for the modal component (we can add this HTML markup in resources/components directory). 
You can then use this component in your views by calling the component's tag and passing in any necessary attributes.

For example, if you generate a "Modal" component with the "php artisan make:component modal" command, you can use it in your views like this:
````
<x-modal title="Example Modal">
    This is the content of the modal.
</x-modal>
````

</details>


<details>

<summary>Database Configuration and Migrations</summary>

Migration reside on the folder database/migrate.

#### setting up the database configuration
In .env file add the database configs.
````
DB_CONNECTION=mysql
DB_HOST=localhost
DB_PORT=3307
DB_DATABASE=learn_laravel
DB_USERNAME=root
DB_PASSWORD=password123
````

#### configure cache
````php artisan config:cache````

#### run migration
````php artisan migrate````

# Create Table Using Migration

#### create migration
````php artisan make:migration create_<table_name>_table````


#### rollback last migration
````php artisan migration:rollback````

#### refresh migration
Deletes all previous migrations and then runs the migration again
````php artisan migration:refresh````

#### adding new columns to table
````php artisan make:migation add_columns_to_<table_name>_table````

</details>



