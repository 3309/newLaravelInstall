# newLaravelInstall

- initiating a new laravel project in a shared web host like godaddy.com
## step one
  - use https://codeanywhere.com/editor/ for online access to server.
  - 'curl -sS https://getcomposer.org/installer | php'     -use this to install latest composer using terminal in codeanywhere. amke sure ssh enabled in server.
  -  'php composer.phar create-project --prefer-dist laravel/laravel blog'  to install the latest laravel application.
  
  -  use Illuminate\Support\Facades\Schema;
      public function boot()
      {
          Schema::defaultStringLength(191);
      }
      you need this for sqldatabase old version. add this in appservice provider.php
      
 - <IfModule mod_rewrite.c>
        RewriteEngine On
        RewriteRule ^(.*)$ public/$1 [L]
    </IfModule> 
    you add this to the root of the application to avoid /public/ in the url.
    
    
-  to install NVM in the godaddy use
   --'curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.31.0/install.sh | bash'
   --*use NVM to install node using 'nvm install node' command
   --make the NPM default with 'nvm alias default node' command -all done.
   --now you can use npm in godaddy
   
