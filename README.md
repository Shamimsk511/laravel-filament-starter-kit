# 🚀 Ercogx Starter Kit

This is a **Filament v3 Starter Kit** for **Laravel 12**, designed to accelerate the development of Filament-powered applications.

![](https://raw.githubusercontent.com/ercogx/laravel-filament-starter-kit/main/preview-white.png)
![](https://raw.githubusercontent.com/ercogx/laravel-filament-starter-kit/main/preview.png)

## 📦 Installation

Follow these steps to install and set up the Laravel Filament Starter Kit.

```bash
laravel new test-kit --using=ercogx/laravel-filament-starter-kit
```

## ⚙️ Setup

1️⃣ **Database Configuration**
- If using **MySQL**, update database credentials in `.env`.

2️⃣ **Run Migrations**
```bash
php artisan migrate
````

3️⃣ Create Filament Admin User
```bash
php artisan make:filament-user
```

4️⃣ Assign Super Admin Role
```bash
php artisan shield:super-admin --user=1 --panel=admin
```

5️⃣ Generate Permissions
```bash
php artisan shield:generate --all --ignore-existing-policies --panel=admin
```

## 🌟Panel Include 

- [Breezy](https://filamentphp.com/plugins/jeffgreco-breezy) My Profile page.
- [Themes](https://filamentphp.com/plugins/hasnayeen-themes) Themes for Filament panels. Setup for `user` mode.
- [Shield](https://filamentphp.com/plugins/bezhansalleh-shield) Access management to your Filament Panel's Resources, Pages & Widgets through spatie/laravel-permission.
- [Settings](https://filamentphp.com/plugins/outerweb-settings) Integrates Outerweb/Settings into Filament.
- [Backgrounds](https://filamentphp.com/plugins/swisnl-backgrounds) Beautiful backgrounds for Filament auth pages.
- [Logger](https://filamentphp.com/plugins/z3d0x-logger) Extensible activity logger for filament that works out-of-the-box.

## 🧑‍💻Development Include

- [barryvdh/laravel-debugbar](https://github.com/barryvdh/laravel-debugbar) The most popular debugging tool for Laravel, providing detailed request and query insights.
- [barryvdh/laravel-ide-helper](https://github.com/barryvdh/laravel-ide-helper) Generates helper files to improve autocompletion and static analysis in IDEs.
- [larastan/larastan](https://github.com/larastan/larastan) A PHPStan extension for Laravel, configured at level 5 for robust static code analysis.

This kit includes **Laravel Pint** for automatic PHP code styling and structured PHPDoc generation for your models.  
After running migrations, execute the following command to update model documentation:

```bash
php artisan ide-helper:models -W && ./vendor/bin/pint app 
```

The `composer check` script runs **tests, PHPStan, and Pint** for code quality assurance:
```bash
composer check
```

## 📜 License

This project is open-source and licensed under the MIT License.

## 💡 Contributing

We welcome contributions! Feel free to open issues, submit PRs, or suggest improvements.


### 🚀 Happy Coding with Laravel & Filament! 🎉
