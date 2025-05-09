# 🚗 Laravel Concessionaria Veicoli Elettrici

[![Laravel](https://img.shields.io/badge/Laravel-10.x-red?style=flat-square&logo=laravel)](https://laravel.com)
[![Dockerized](https://img.shields.io/badge/Docker-Supported-blue?style=flat-square&logo=docker)](https://www.docker.com)
[![License](https://img.shields.io/badge/license-MIT-green.svg?style=flat-square)](LICENSE)

Sistema gestionale per una **concessionaria di veicoli elettrici**, sviluppato in Laravel con supporto per **Docker**, **Herd**, e funzionalità avanzate come autenticazione API, gestione immagini e dashboard per noleggi.

---

## 🔧 Stack Tecnologico

- **Backend:** Laravel 10+, PHP 8.2
- **Frontend:** Blade, TailwindCSS
- **Autenticazione:** Laravel Sanctum
- **Ambiente locale:** [Herd](https://herd.dev)
- **Containerizzazione:** Docker, Nginx
- **Database:** MySQL / MariaDB
- **Build Assets:** Vite (Node.js)

---

## 🚀 Funzionalità Chiave

### 🧍 Utenti
- Registrazione/Login protetto (Sanctum)
- Logout globale da tutti i dispositivi
- Ruoli utente (admin/user)

### 🚘 Veicoli
- CRUD completo
- Upload e gestione immagini
- Associazione tag ai veicoli
- API RESTful con Resource personalizzate
- Validazioni avanzate con `FormRequest`

### 🛒 Noleggi
- Gestione noleggi clienti
- Visualizzazione con date formattate
- Statistiche e miglioramenti UI

### 🔒 Sicurezza
- Middleware protetti con token API
- Protezione rotte
- Gestione permessi

---

## 📦 Docker & Deploy

È incluso un ambiente **completo e pronto al deploy** tramite Docker:

- **Nginx** configurato
- **Dockerfile** ottimizzato
- **Node.js build** per asset
- **Permessi e volumi** configurati

```bash
# Build del container
docker-compose up --build

# Accesso container Laravel
docker exec -it app bash
