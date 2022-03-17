# https://www.youtube.com/watch?v=hOF2NQkkyYk


laravel new projectname
composer install
php artisan key:generate

php artisan serve

composer require laravel/ui
//instaling view component

php artisan ui vue --auth
//now if we refresh page we have login and register page ready



npm install laravel-mix@latest
npm install vue-loader
npm install && npm run dev


xampp running DB
create new DB laravel_shop

php artisan migrate

# 11:03 installing theme
ctrl+c content of index into the product
copy assets folder into public folder

copy auth code into navigation
@if (Route::has('login'))
    <div class="hidden fixed top-0 right-0 px-6 py-4 sm:block">
        @auth
            <a href="{{ url('/home') }}" class="text-sm text-gray-700 dark:text-gray-500 underline">Home</a>
        @else
            <a href="{{ route('login') }}" class="text-sm text-gray-700 dark:text-gray-500 underline">Log in</a>

            @if (Route::has('register'))
                <a href="{{ route('register') }}" class="ml-4 text-sm text-gray-700 dark:text-gray-500 underline">Register</a>
            @endif
        @endauth
    </div>
@endif

# 14:45