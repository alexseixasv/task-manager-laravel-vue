# Task Manager - Laravel 10 & Vue 3

A full-stack task management application built with **Laravel 10**, **Vue 3**, **Inertia.js**, **PostgreSQL**, **Pinia**, and **Pest**.  
This project was created as part of a technical assessment to demonstrate full-stack development skills, API design, and frontend reactivity using modern tools.

---

## ⚙️ Stack

- **Backend**: Laravel 10 (PHP 8.2+)
- **Frontend**: Vue.js 3 with Inertia.js
- **State Management**: Pinia 2.0
- **Database**: PostgreSQL 15
- **Testing**: Pest 2.0

---

## 🚀 Setup Instructions

1. **Clone the repository**  
   ```bash
   git clone https://github.com/alexseixasv/task-manager-laravel-vue.git
   cd task-manager-laravel-vue
   ```

2. **Install PHP and JavaScript dependencies**  
   ```bash
   composer install
   npm install
   ```

3. **Create and configure `.env` file**  
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

   Update your `.env` with PostgreSQL settings:
   ```env
   DB_CONNECTION=pgsql
   DB_HOST=127.0.0.1
   DB_PORT=5432
   DB_DATABASE=taskmanager
   DB_USERNAME=your_user
   DB_PASSWORD=your_password
   ```

4. **Run migrations and seeders**
   ```bash
   php artisan migrate --seed
   ```

5. **Start development servers**
   ```bash
   php artisan serve
   npm run dev
   ```

---

## 📐 Architectural Notes

- **Inertia.js** is used to bridge Laravel (backend) and Vue (frontend) in a monolithic SPA architecture.
- **Pinia** is used for state management across Vue components.
- **Pest** is used for expressive, modern testing (unit + feature).
- Routes and controllers follow RESTful conventions.
- Request validation is handled via Form Requests.

---

## ✅ Assumptions

- Users are authenticated (auth scaffolding can be assumed or stubbed).
- Tasks are basic CRUD entities with soft delete and restore.
- Task updates could use Laravel Echo for real-time feedback (bonus).

---

## 🧪 Running Tests

```bash
php artisan test
# or
./vendor/bin/pest
```

---

## 📄 License

This project is for technical evaluation purposes only.
