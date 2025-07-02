# BestWeb-Tech---Laravel-Test-SIT-BOON-LIANG-

# Laravel Product CRUD API

## Requirements
- PHP >= 8.1
- Composer
- MySQL

## Setup
```bash
git clone <repo>
cd <project>
composer install
cp .env.example .env
php artisan key:generate
```

Configure `.env` for DB connection.

```bash
php artisan migrate
```

(Optional) Create a personal access token if using Sanctum.

## API Endpoints
| Method | Endpoint                     | Description                |
|--------|------------------------------|----------------------------|
| GET    | /api/products                | List products              |
| POST   | /api/products                | Create product             |
| GET    | /api/products/{id}           | Show product               |
| PUT    | /api/products/{id}           | Update product             |
| DELETE | /api/products/{id}           | Soft delete product        |
| POST   | /api/products/bulk-delete    | Bulk delete                |
| GET    | /api/products-export         | Export to Excel            |

## Testing
```bash
php artisan test
```

## Docker
If implemented, see `docker-compose.yml`.

## Notes
- Authentication: Laravel Sanctum
- Exports: Laravel Excel
- Validation: Form Requests
