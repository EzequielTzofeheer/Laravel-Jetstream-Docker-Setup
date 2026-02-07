# Laravel Jetstream Docker Setup

![Laravel](https://img.shields.io/badge/Laravel-12.x-red)
![PHP](https://img.shields.io/badge/PHP-8.3%2B-blue)
![Docker](https://img.shields.io/badge/Docker-Ready-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Stable-success)

A **Docker-based, reusable and standardized development environment** for **Laravel 12 + Jetstream**, focused on productivity, consistency and best practices.

---

## 📌 What is this?

**Laravel Jetstream Docker Setup** is a boilerplate repository that provides a complete local development environment for **Laravel 12** using **Docker** and **Docker Compose**.

It delivers a ready-to-use infrastructure with all essential services preconfigured, allowing developers to focus on building features instead of setting up environments.

---

## 🎯 What is it for?

This project is intended to be used as a **starting point** for new Laravel applications that require:

- A fully configured Docker environment
- Consistent setup across multiple projects
- Faster onboarding for new developers
- Reduced time spent on infrastructure configuration
- Clean and predictable project structure

Ideal for both **teams and solo developers** who value reproducibility and scalability.

---

## 🧠 How does it work?

The environment uses **Docker Compose** to orchestrate multiple containers, each with a clear responsibility:

- **App**: PHP container where the Laravel application runs
- **Queue**: Dedicated worker container for processing Laravel queues
- **Nginx**: Web server responsible for handling HTTP requests
- **MySQL**: Relational database
- **Redis**: Cache and queue backend
- **PHPMyAdmin**: Web interface for database management

All services communicate through a dedicated Docker bridge network.

---

## 🚀 Quick Installation

### 1️⃣ Clone the repository

```bash
git clone https://github.com/EzequielTzofeheer/Laravel-Jetstream-Docker-Setup
```

2️⃣ Access the project directory

```bash
cd Laravel-Jetstream-Docker-Setup
```

3️⃣ Create the environment file

```bash
cp .env.example .env
```

4️⃣ Build and start the containers

```bash
sudo docker compose up -d
```

5️⃣ Access the Docker container

```bash
sudo docker compose exec app bash
```

6️⃣ Install Laravel dependencies

```bash
composer install
```

7️⃣ Generate the application key

```bash
php artisan key:generate
```

8️⃣ Run the database migrations

```bash
php artisan migrate
```

9️⃣ Install the Node.js dependencies using NPM

```bash
npm install
```

9️⃣ Compile and optimize frontend assets for development or production:

```bash
npm run build
```

---

## 🌐 Access

- Application: http://localhost:8093
- PhpMyAdmin: http://localhost:8553

---

## 🎯 Goal / Purpose

The main goals of this repository are:

- Provide a standardized Laravel + Docker setup
- Serve as a reusable base for multiple projects
- Improve development speed and consistency
- Avoid repetitive manual environment setup
- Use tags for versioning instead of branches

This repository is not a final product, but a solid foundation to build upon.

---

## 🧱 Tech Stack

- PHP 8.3+
  - Laravel 12.x
  - Jetstream
- Docker
  - Docker Compose 
- Nginx
- MySQL 8
- Redis
- PHPMyAdmin

---

## 🧩 Compatibility

- PHP: 8.3 or higher
- Laravel: 12.x
- Docker: 24 or higher
- Docker Compose: 2.x or higher
- Supported operating systems:
  - Linux
  - macOS
  - Windows (WSL2)

---

## 🤝 Contributing

Contributions are welcome.

You can contribute by:

- Opening issues
- Submitting pull requests
- Suggesting improvements to the setup or documentation

Please ensure all contributions remain generic, reusable and framework-agnostic where possible.

---

## 🙌 Credits

- Laravel Framework
- Docker
- Open Source Community

---

## ⭐ Support

If this repository was useful to you, consider leaving a ⭐ on GitHub.

It helps support the project and encourages continuous improvement.

---

## 👤 Author

Developed and maintained by **Ezequiel Tzofeheer**

**Full Stack Developer** with a strong focus on building clean, scalable and secure applications.

**Core areas of focus**

- Clear and maintainable architecture
- High productivity and developer experience
- Cyber security and data protection
- Software engineering best practices
- Performance and cost efficiency

---

📄 License

This project is licensed under the MIT License.

See the LICENSE file for more details.
