<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## Installation

Instala las dependencias con Composer
- composer install
- npm i ó npm install, para dependencias extras.

Copia el archivo .env.example a uno nuevo archivo .env ( Asegurarse de colocar los datos de la conexion a base de datos)
- cp .env.example .env

Generar la clave para la aplicación
- php artisan key:generate

Ejecutar las migraciones
- php artisan migrate

Ejecutar los seeders
- php artisan db:seed

Realizar estos pasos, en caso tal que presenete problemas o cada vez que se ejecute una acción (opcional)
- php artisan cache:clear
- php artisan config:clear
- php artisan route:clear
- php artisan view:clear

Si se va a trabajar en un entorno windows, el comando se puede utilizar a traves de un programador de tareas.
- 1. Dirigirse al programador de tareas.
- 2. En acciones seleccionar, crear tarea.
- 3. En general colocarle un nombre, para identificarla.
- 4. En desencadenadores especificar cada cuanto desean que se ejecute el comando.
- 5. En acciones, como accion selecionaran "Iniciar un programa".
- 6. En acciones, como programa o script, colocaran la ruta de su ejecutable de php algo como esto "C:\xampp\php\php.exe".
- 7. En acciones, en agregar argumentos, colocaran la ruta de su proyecto seguido del comando, deberia verse algo asi "C:\xampp\htdocs\Proyecto-api-wordpress\artisan sync:orders"
- 8. En acciones, en iniciar en, colocaran la ruta de su proyecto, deberia verse algo asi "C:\xampp\htdocs\Proyecto-api-wordpress"

En Linux:
- Traslada la configuración del comando de Kernel.php a routes/console.php, ya que Laravel 11 dejó de utilizar Kernel para estos comandos en tareas programadas.
- Modifica la lógica de tiempo dentro de app\Console\Commands\SyncOrderToErpc.php.
- Configura el CRON en tu sistema para que ejecute php artisan schedule:run


Para iniciar el proyecto:
Para el frontend (Vite)
- npm run dev

Para el backend (Laravel)
- php artisan serve

Ambos deben estar iniciados en el mismo momento, cada una en su respectiva terminal, claro esta.


## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains thousands of video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the [Laravel Partners program](https://partners.laravel.com).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[WebReinvent](https://webreinvent.com/)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[DevSquad](https://devsquad.com/hire-laravel-developers)**
- **[Jump24](https://jump24.co.uk)**
- **[Redberry](https://redberry.international/laravel/)**
- **[Active Logic](https://activelogic.com)**
- **[byte5](https://byte5.de)**
- **[OP.GG](https://op.gg)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
