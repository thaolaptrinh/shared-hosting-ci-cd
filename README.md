# Shared Hosting CI/CD Demo

A collection of demo applications demonstrating CI/CD pipeline for shared hosting deployment with different frameworks.

## Project Structure

```
shared-hosting-ci-cd/
├── .github/workflows/    # GitHub Actions workflows
│   ├── deploy-php.yml    # PHP deployment workflow
│   ├── deploy-node.yml   # Node.js deployment workflow
│   └── deploy-laravel.yml # Laravel deployment workflow
├── src_demos/            # Demo applications source code
│   ├── php/             # Simple PHP application
│   ├── node/            # Node.js Express application
│   └── laravel/         # Laravel application
├── scripts/             # Deployment scripts
└── README.md           # Project documentation
```

## Demo Applications

### 1. PHP Demo
A simple PHP application demonstrating basic CI/CD workflow.

```bash
cd src_demos/php
composer install
php -S localhost:8000
```

### 2. Node.js Demo
A Node.js Express application with basic API endpoints.

```bash
cd src_demos/node
npm install
npm start
```

### 3. Laravel Demo
A Laravel application with full features.

```bash
cd src_demos/laravel
composer install
php artisan serve
```

## CI/CD Pipeline

Each demo application has its own workflow:

1. **PHP Demo**
   - Build and test PHP application
   - Deploy to shared hosting using FTP
   - Verify deployment

2. **Node.js Demo**
   - Install dependencies
   - Run tests
   - Build application
   - Deploy to shared hosting

3. **Laravel Demo**
   - Install Composer dependencies
   - Run tests
   - Build assets
   - Run migrations
   - Deploy to shared hosting

## Environment Variables

Each demo application requires its own environment variables. Check the respective `.env.example` files in each demo directory.

## Deployment

Applications are automatically deployed to shared hosting when changes are pushed to the main branch. Each application has its own deployment script and workflow.

## License

MIT