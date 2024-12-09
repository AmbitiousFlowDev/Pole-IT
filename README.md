# Pole-IT

![Laravel](https://img.shields.io/badge/Laravel-10.x-red)
![SQLite](https://img.shields.io/badge/SQLite-3-blue)
![Filament](https://img.shields.io/badge/Filament-2.x-green)
![Livewire](https://img.shields.io/badge/Livewire-2.x-orange)

---

## Project Structure

### Key Directories
- **`app`**: Contains the core application logic, including resources, controllers, and models.
  - **`Filament/Resources`**: Defines Filament resources like `ActivityResource`, `BlogResource`, `ProductResource`, etc.
  - **`Http/Controllers`**: Houses application controllers.
  - **`Models`**: Contains Eloquent models.
  - **`Providers`**: Includes custom service providers.
- **`config`**: Application configuration files.
- **`database`**: Database migrations, factories, and seeders.
- **`public`**: Publicly accessible assets such as CSS, JavaScript, and images.
- **`resources`**: Contains front-end resources like views, CSS, and JavaScript.
  - **`views`**: Includes Blade templates for pages like `auth`, `home`, and `shop`.
- **`routes`**: Contains route definitions.
- **`storage`**: Stores files, logs, and cache data.
- **`tests`**: Automated tests for the application.

---

## Features

- **Filament Admin Panel**: Manage resources such as products, orders, and blogs.
- **Livewire Integration**: Build reactive and dynamic front-end components.
- **SQLite Database**: Lightweight database for quick setup and development.
- **Customizable Views**: Organized templates for pages like the shop and home.

---

## Installation

1. **Clone the repository**:
   ```bash
   git clone <repository_url>
   cd <project_directory>
   ```

2. **Install dependencies**:
   ```bash
   composer install
   npm install
   ```

3. **Set up environment variables**:
   Copy `.env.example` to `.env` and configure it for SQLite:
   ```env
   DB_CONNECTION=sqlite
   DB_DATABASE=database/database.sqlite
   ```

   Create the SQLite database file:
   ```bash
   touch database/database.sqlite
   ```

4. **Run migrations**:
   ```bash
   php artisan migrate --seed
   ```

5. **Start the development server**:
   ```bash
   php artisan serve
   npm run dev
   ```

---

## Usage

- Access the application via the URL provided by `php artisan serve`.
- Use the Filament admin panel for resource management (`/admin` by default).

---

## Testing

Run automated tests to ensure the application is functioning as expected:
```bash
php artisan test
```

---

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue for bug fixes or feature requests.

---

## License

This project is open-source and available under the [GNU LICENSE](LICENSE).

--- 

Feel free to adjust as per your needs!
