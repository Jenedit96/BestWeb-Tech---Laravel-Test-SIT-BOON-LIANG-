# BestWeb-Tech---Laravel-Test-SIT-BOON-LIANG-

# Laravel Product CRUD API

## Setup

```bash
git clone <repository_url>
cd <project>
composer install
cp .env.example .env
php artisan key:generate
```

Configure `.env` with MySQL credentials.

Run migrations:

```bash
php artisan migrate
```

(Optional) Seed data:

```bash
php artisan db:seed
```

## API Endpoints

| Method | Endpoint                | Description                      |
|--------|-------------------------|----------------------------------|
| GET    | /api/products           | List products                    |
| POST   | /api/products           | Create product                   |
| GET    | /api/products/{id}      | Show product details             |
| PUT    | /api/products/{id}      | Update product                   |
| DELETE | /api/products/{id}      | Soft delete product              |
| POST   | /api/products/bulk-delete | Bulk delete products           |

## Running Tests

```bash
php artisan test
```

## Docker (Optional)

See `docker-compose.yml` for Docker setup instructions.

## Assumptions and Design Choices

- Used Laravel Sanctum for authentication.
- Soft deletes implemented via Eloquent.
- Validation via Form Requests.
- Pagination defaults to 10 items per page.
