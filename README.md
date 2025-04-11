# 💡 Billify — ISP Billing Management App

**Billify** is a billing management application built using Laravel and FilamentPHP. Originally designed for [Fyui.Net](https://fyui.net), it is also suitable for other Internet Service Providers (ISPs) with similar billing systems and workflows.

## 🚀 Features

- Customer management
- Monthly billing generation
- Payment status tracking
- WhatsApp notifications for due invoices
- Role-based access control (via Filament)
- Token-based API authentication for client-side apps
- Automatic service restriction for unpaid customers
- Dashboard with key billing and customer metrics

## 🧰 Tech Stack

- **Backend**: Laravel 11
- **Admin Panel**: FilamentPHP (with [filament-starter](https://github.com/ryangjchandler/filament-starter))
- **Frontend**: Blade, Livewire, TailwindCSS
- **Database**: MySQL
- **Messaging Integration**: WhatsApp API
- **Client Verification**: REST API with token validation

## ⚙️ Installation

```bash
git clone https://github.com/fyutaru-dev/billify.git
cd billify
cp .env.example .env
composer install
php artisan key:generate
php artisan migrate --seed
php artisan storage:link
npm install && npm run build
```

## 🧪 Development

To run the app locally:

```bash
php artisan serve
```

Login to Filament Admin at `http://localhost:8000/admin` using the seeded credentials.

## 🔐 Default Admin Credentials (for testing)

```
Email: admin@fyui.net
Password: password
```

> ⚠️ Make sure to change the default password after login.

## 📦 API Integration (Token Auth)

Billify exposes a token-based API for client applications. Each customer is assigned a token which is verified via the API to validate access.

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repository and submit a pull request.

## 📄 License

This project is licensed under the MIT License.


Built with ❤️ by [PT.Fyui Digital Nusantara](https://fyui.net)
