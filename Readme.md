# Max Smeele Portfolio – Technical Samples

**ES:**  
Este repositorio contiene una versión pública y documentada del portfolio de Max Smeele.  
Nota: Debido a acuerdos de confidencialidad, este código es una exhibición de la arquitectura y componentes técnicos; la lógica de negocio privada y configuraciones sensibles permanecen en un repositorio privado.

**EN:**  
This repository contains a public, documented version of Max Smeele's portfolio.  
Note: Due to confidentiality agreements, this code serves as a technical showcase of architecture and components; private business logic and sensitive configurations remain in a private repository.

---

## Índice / Table of Contents

- [Descripción general / Overview](#descripción-general--overview)
- [Tecnologías / Technologies](#tecnologías--technologies)
- [Estructura del proyecto / Project-structure](#estructura-del-proyecto--projects-structure)
- [Instalación / Installation](#instalación--installation)
- [Uso / Usage](#uso--usage)
- [Despliegue / Deployment](#despliegue--deployment)
- [Contribuir / Contributing](#contribuir--contributing)
- [Créditos / Credits](#créditos--credits)
- [Licencia / License](#licencia--license)

---

## Descripción general / Overview

**ES:**  
Este proyecto es el portfolio digital de alta performance para Max Smeele, diseñado para la difusión científica y fotográfica.  
La solución emplea un backend robusto en Django y un frontend dinámico en Vue 3, sincronizados mediante una API REST (Django REST Framework) optimizada para la carga de contenido multimedia pesado sin comprometer el SEO técnico.

**EN:**  
This project is a high-performance digital portfolio for Max Smeele, designed for scientific and photographic dissemination.  
The solution uses a robust Django backend and a dynamic Vue 3 frontend, synchronized via a REST API (Django REST Framework) optimized for handling heavy multimedia content without compromising technical SEO.

---

## Tecnologías / Technologies

- **Backend:** Django 4.2+, Django REST Framework, PostgreSQL, Gunicorn
- **Frontend:** Vue 3 (Composition API), PrimeVue, Vite, Sass
- **DevOps & Otros / Other:** Docker, Docker Compose, Nginx, python-dotenv, Pillow (Image Processing)

---

## Estructura del proyecto / Project Structure

```
/
|-- backend/           # Lógica del servidor y API REST / Server logic & REST API
|   |-- requirements.txt
|   |-- manage.py
|-- frontend/          # Interfaz de usuario reactiva / Reactive User Interface
|   |-- src/
|   |-- public/
|   |-- README.md
|-- scripts/
|   |-- deploy.sh      # Script de automatización (CI/CD parcial) / Automation script
|-- docker-compose.prod.yml
```

---

## Instalación / Installation

### Prerrequisitos / Prerequisites

- Python 3.12+
- Node.js >= 16
- Docker & Docker Compose (Recomendado para producción / Recommended for production)

### Backend Setup

```bash
cd backend
python -m venv venv
source venv/bin/activate  # (Linux/Mac)
venv\Scripts\activate     # (Windows)
pip install -r requirements.txt
```
Configura el archivo `.env` basándote en la plantilla de ejemplo proporcionada.  
Configure the `.env` file based on the provided example template.

### Frontend Setup

```bash
cd frontend
npm install
```

---

## Uso / Usage

### Desarrollo / Development

**Backend:**
```bash
python manage.py migrate
python manage.py runserver
```

**Frontend:**
```bash
npm run dev
```

---

## Despliegue / Deployment

El despliegue está automatizado mediante contenedores Docker y un script bash especializado para gestionar migraciones y builds de forma atómica.  
Deployment is automated via Docker containers and a specialized bash script to handle migrations and builds atomically.

```bash
chmod +x scripts/deploy.sh
./scripts/deploy.sh --full
```

---

## Contribuir / Contributing

Las contribuciones externas no están habilitadas en esta edición pública.  
External contributions are not enabled in this public edition.

---

## Créditos / Credits

- **Cliente / Client:** Max Smeele  
- **Desarrollo Técnico / Lead Developer:** RubenVSM

---

## Licencia / License

**ES:**  
Este código se distribuye únicamente con fines de exhibición técnica. Todos los derechos sobre la marca y el contenido visual pertenecen al cliente. Consulte con los autores antes de cualquier reutilización.

**EN:**  
This code is distributed for technical showcase purposes only. All rights regarding branding and visual content belong to the client. Please contact the authors before any reuse.

**Estado del Proyecto:**  
Producción (Repositorio original alojado en servidor privado)  
Production status (Original repository hosted on a private server)
