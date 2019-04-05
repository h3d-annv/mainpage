1. Clone the project in the www folder
    ```
    git clone https://github.com/h3d-anhnq/DemoOctoberCMS.git
    ```

1. Install dependencies
	```
	composer install
	```
	
1. Create env file
	```
	php artisan october:env
	```
	
1. Change mysql config in env file
	```
	DB_CONNECTION=mysql
	DB_HOST=your_mysql_host (Default localhost)
	DB_PORT=your_mysql_port (Default 3306)
	DB_DATABASE=your_database_name
	DB_USERNAME=your_mysql_username
	DB_PASSWORD=your_mysql_password
	```

1. (Optional if you want different account name and password) Change default admin account in /modules/backend/database/seeds/SeedSetupAdmin.php 

1. Run migration
    ```
    php artisan october:up
    ```

1. (If admin account is not created) Run seed for admin account
   ```
   php artisan db:seed --class=\Backend\Database\Seeds\SeedSetupAdmin
   ```
#   m a i n p a g e  
 #   m a i n p a g e  
 