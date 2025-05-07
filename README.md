# 🗂️ Task Manager — Full Stack Laravel + Vue 3 + Inertia

This is a full-stack monolithic SPA built with Laravel 10, Vue.js 3, and Inertia.js. The backend is powered by Laravel, while the frontend uses Vue.js with Vite as the build tool.

---

## 📦 Tech Stack

- **Laravel 10** — backend framework
- **Vue.js 3** — frontend reactive components
- **Inertia.js** — client-side routing in a monolith setup
- **Vite** — lightning-fast frontend build tool
- **PostgreSQL 15** — relational database
- **Pinia 2.0** — state management for Vue
- **Pest 2.0** — testing framework

---

## 🚀 Getting Started

### Requirements

- PHP >= 8.2
- Composer
- Node.js >= 18
- PostgreSQL 15

### Setup Instructions

```bash
# Install PHP dependencies
composer install

# Install JavaScript dependencies
npm install

# Create .env file
cp .env.example .env

# Generate app key
php artisan key:generate

# Set database credentials in .env
# Then run migrations
php artisan migrate

# Start dev servers
npm run dev
php artisan serve
```

---

## 🧰 Local Development (Windows with Laragon)

If you're on Windows, you can run this project using [Laragon](https://laragon.org/), which includes PHP, Composer, Node.js, and PostgreSQL out of the box.

After installing Laragon:

```bash
# Open Laragon Terminal and navigate to project folder
cd D:\Repositorios\task-manager-laravel-vue

# Run backend and frontend
composer install
npm install
php artisan migrate
php artisan serve
npm run dev
```

---

## 📁 Project Structure

- `app/` – Laravel backend logic (controllers, models)
- `routes/web.php` – Routes using Inertia + Vue
- `resources/js/Pages` – Vue components (Inertia pages)
- `resources/views/app.blade.php` – Root layout (Inertia)
- `vite.config.js` – Vite + Vue config
- `tests/` – Pest or PHPUnit tests (empty by default)

---

## 🧪 Testing

```bash
# Run test suite (after installing Pest)
php artisan test
```

---

## 📝 Assumptions

- The project is a monolithic SPA using Laravel + Vue via Inertia.
- PostgreSQL is used as the database.
- The frontend is served via Vite and Vue 3 using Inertia pages.

---