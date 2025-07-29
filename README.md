# 🏗️ LoteSmart

**LoteSmart** is a web-based land lot sales and management platform built with Laravel.  
It helps real estate developers and sales teams streamline the lot reservation process, payment tracking, and user roles administration.

## 🚀 Features

- Project > Stage > Lot structure management
- Role-based access: Super Admin, Admin, Seller, Client
- Monthly payment tracking system
- Interest on late payments
- Lot reservation and sales tracking
- Notifications via Laravel Reverb (WebSockets)
- Responsive design (Bootstrap 5)
- Docker-ready for local development and production

## 🧱 Tech Stack

- Laravel 11 (PHP 8.3+)
- MySQL
- Bootstrap 5
- Laravel Reverb (WebSockets)
- Docker (Laradock)
- NGINX + HTTPS (Production-ready)

## 📦 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/lotesmart.git
   cd lotesmart
2. Copy and configure environment:
   ```bash
   cp .env.example .env
3. Install dependencies:
   ```bash
   composer install
   npm install && npm run build
4. Run database migrations:
   ```bash
   php artisan migrate --seed
5. Start development server:
   ```bash
   php artisan serve
Note: For Docker setup using Laradock, see /docs/docker-setup.md (coming soon).

📁 Project Structure

lotesmart/
├── app/
├── bootstrap/
├── config/
├── database/
├── public/
├── resources/
├── routes/
├── storage/
└── tests/

👥 Roles Overview
| Role        | Capabilities                                                   |
| ----------- | -------------------------------------------------------------- |
| Super Admin | Full system access, user and project management                |
| Admin       | Manages developments, lots, and payment plans                  |
| Seller      | Reserves and sells lots, views client payments                 |
| Client      | Views their own purchases, payment schedule, and notifications |

📝 License
This project is open-source and available under the MIT License.
