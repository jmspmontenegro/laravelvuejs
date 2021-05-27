## ❓ About this project

This repository is simple but helps me to remember the easy steps to starting a project Laravel + Vue.js.


## ❤ Instaling Laravel and Vue.js with Laravel/ui

- Create the Laravel project on the last version:
```
composer create-project --prefer-dist laravel/laravel
```
- Open created directory and install Laravel/UI package. It is an extraction of the frontend of Laravel on a separated package which helps the development of front isolated of main Laravel code. 
```
composer require laravel/ui
```
- Previously, Laravel has templates of login files but after the 5.1 version, all of them were removed, and to install it again need to execute the commando below. And this is perfect because we can choose others frontend frameworks like Bootstrap or React. This is really the simplest explanation, so I recommend read more about it.
```
php artisan ui vue
```
- NPM is a package manager, and the below command will install all necessary packages to the project work. If you use Yarn use a similar command. 
```
npm i
```
- Is necessary to build, which means create minified files of JS and CSS files and put them in the PUBLIC directory.
```
npm run dev
```
## ❗ After install, change the *welcome* page

To test it working, we can change the welcome.blade.php file inserting the link to app.css and app.js built. And using the example component too. 
```
<!DOCTYPE html>
<html lang="{{ str_replace('_', '-', app()->getLocale()) }}">
    <head>
        <meta charset="utf-8">
        <meta name="viewport" content="width=device-width, initial-scale=1">

        <title>Laravel+Vue.js</title>

        <link rel="stylesheet" href="{{asset('css/app.css')}}">
    </head>
    <body class="antialiased">

        <div id="app">
            <example-component></example-component>
        </div>

        <script src="{{asset('js/app.js')}}"></script>
    </body>
</html>
```
## 🚀 And that is all folks!

So, that is really easy! Now, you can clone the folder but better do all these steps yourself. :) 