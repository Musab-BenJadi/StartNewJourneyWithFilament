# mu_app (Laravel + Filament)

I'm Starting new journey with Filament Laravel Package.

## About
Lightweight Laravel app using Filament admin panel for content and admin management.

## Prerequisites
- PHP 10.0+
- Composer
- Node.js 16+ and npm or yarn
- Git
- MySQL / PostgreSQL (or other supported DB)
- (Optional) Docker / Laravel Sail for containerized dev

## Clone repository
- HTTPS:
    git clone https://github.com/Musab-BenJadi/StartNewJourneyWithFilament.git

## Local setup
1. Enter project
     cd mu_app
2. Copy env and generate key
     cp .env.example .env
     composer install
     npm install
     npm run dev     # or `npm run build` for production assets
     php artisan key:generate
3. Configure .env (DB, mail, etc.)
4. Run migrations & seeders
     php artisan migrate --seed
5. Link storage (if used)
     php artisan storage:link
6. Create admin user (Filament)
     php artisan make:filament-user
7. Serve app
     php artisan serve
     # or use `./vendor/bin/sail up -d` if using Sail/Docker

## Filament notes
- See Filament Docs: https://filamentphp.com/docs
- Admin panel available at /admin (or configured route).
- Use `php artisan make:filament-user` to create an admin account for Filament.
- Check config/filament.php for customizations.

## Dev tools used
- VS Code (with PHP Intelephense, Tailwind CSS IntelliSense)
- PHPStorm (optional)
- Laravel Valet or Sail / Docker
- Xdebug for step debugging
- Git for version control
- Node/npm or yarn for front-end builds
- Laravel Telescope (optional for debugging)
- Laravel Debugbar (optional)

