# Laravel Job Management App

A web application built with the Laravel PHP framework to manage job entries and user authentication. This project showcases CRUD operations, background job processing, and route/controller architecture using Laravel.

---

## Table of Contents

-   [Project Structure](#project-structure)
-   [Features](#features)
-   [Installation](#installation)
-   [How to Use](#how-to-use)
-   [Available Routes](#available-routes)
-   [Requirements](#requirements)
-   [Contribution](#contribution)
-   [Learn More](#learn-more)

---

## Project Structure

```
demo_laravel/
├── app/Http/Controllers/     # Application controllers
├── app/Jobs/                 # Background job classes (e.g., TranslateJob)
├── database/migrations/      # DB migration files
├── routes/web.php            # Web routes
├── resources/views/          # Blade templates
├── .env.example              # Example environment file
├── composer.json             # PHP dependencies
├── artisan                   # Laravel CLI tool
```

---

## Features

-   Full CRUD for job entries
-   User authentication (registration & login)
-   RESTful routing using Laravel's web routes
-   Environment configuration with `.env` file

---

## Installation

1. **Clone the repository:**

    ```bash
    git clone git@github.com:LSCasas/demo_laravel.git
    cd demo_laravel
    ```

2. **Install dependencies:**

    ```bash
    composer install
    ```

3. **Set up the environment file:**

    ```bash
    cp .env.demo_laravel .env
    ```

    Then update `.env` with your database credentials and app configuration.

4. **Generate application key:**

    ```bash
    php artisan key:generate
    ```

5. **Run database migrations:**

    ```bash
    php artisan migrate
    ```

6. **Start the development server:**

    ```bash
    php artisan serve
    ```

---

## How to Use

You can access the application in your browser via:

```
http://localhost:8000
```

Make sure your database is properly configured and migrated.

---

## Available Routes

### Public Pages

-   Home: `/`
-   Contact: `/contact`

### Jobs Module

-   List all jobs: `/jobs`
-   Create new job: `/jobs/create`
-   Edit existing job: `/jobs/{job}/edit`

### Authentication

-   Register: `/register`
-   Login: `/login`

---

## Requirements

-   PHP 8.x
-   Laravel 10.x
-   Composer
-   MySQL or another compatible relational DBMS

---

## Contribution

1. Fork the repository

2. Create a new branch:

    ```bash
    git checkout -b feature/my-feature
    ```

3. Commit your changes:

    ```bash
    git commit -am "Add new feature"
    ```

4. Push your changes:

    ```bash
    git push origin feature/my-feature
    ```

5. Open a Pull Request

---

## 📚 Learn More

-   [Laravel Documentation](https://laravel.com/docs)
-   [Composer](https://getcomposer.org/)
-   [Laravel Queues & Jobs](https://laravel.com/docs/queues)
-   [Blade Templates](https://laravel.com/docs/blade)

---

Your feedback and contributions are welcome!
