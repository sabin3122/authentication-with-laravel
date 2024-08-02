# Laravel Authentication Project

## Overview

This project demonstrates user authentication using Laravel. It includes user registration, login, password reset, and email verification features. This setup uses Laravel's built-in authentication system, Vue.js for the frontend (optional), and is suitable for learning and development purposes.

## Features

- **User Registration**: Allows users to create an account.
- **Login**: Users can log in to their accounts.
- **Password Reset**: Users can reset their passwords if forgotten.
- **Email Verification**: Optionally verify user emails upon registration.
- **Vue.js Integration**: Optional frontend framework setup.

## Prerequisites

- PHP (7.4 or higher)
- Composer
- Node.js and npm (for frontend dependencies)
- MySQL or another supported database

## Installation

1. **Clone the Repository**

    ```bash
    git clone https://github.com/sabin3122/authentication-with-laravel.git
    cd authentication-with-laravel
    ```

2. **Install Dependencies**

    Install PHP and Laravel dependencies:

    ```bash
    composer install
    ```

    Install JavaScript dependencies (if using Vue.js):

    ```bash
    npm install
    ```

3. **Configure Environment**

    Copy the example environment file and edit it:

    ```bash
    cp .env.example .env
    ```

    Update the `.env` file with your database and mail server configurations.

4. **Generate Application Key**

    ```bash
    php artisan key:generate
    ```

5. **Run Migrations**

    Set up the database schema:

    ```bash
    php artisan migrate
    ```

6. **Compile Assets** (if using Vue.js)

    ```bash
    npm run dev
    ```

## Usage

1. **Run the Development Server**

    ```bash
    php artisan serve
    ```

    The application will be available at `http://localhost:8000`.

2. **Access the Application**

    - Register a new user at `http://localhost:8000/register`.
    - Log in with the registered user at `http://localhost:8000/login`.

## Testing

To test the application, use the following command to run the tests:

```bash
php artisan test
