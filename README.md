## ❓ About this project

This repository is simple, but help me to remeber this easy steps to starting a project Laravel + Vue.js.


## ❤ Instaling Laravel and Vue.js with Laravel/ui

- Create the Laravel project on the last version:
```
composer create-project --prefer-dist laravel/laravel
```
- Open created directory and install Laravel/UI package. It is a extration of the frontend of Laravel on a separated package and this helps the development of front isolated of main Laravel code. 
```
composer require laravel/ui
```
- NPM is a package manager, and the below command will install all necessery packages to the project work. 
```
npm i
```
- So, is necessary make the build , it means create minified files of all *js* and *css* files and put them on *public* directory.
```
npm run dev
```
## ❗ After install, change the *welcome* page

To test it working, we can change welcome.blade.php file inserting the link to app.css and app.js builded. And using the example component too. 
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

So, that is really easy! Now, you can clone the folder but I better do all this steps yourself. :) 