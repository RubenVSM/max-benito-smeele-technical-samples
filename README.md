# Max Benito Smeele - Technical Samples

Technical showcase of a high-performance portfolio developed with **Django (DRF)** and **Vue 3**. Focused on multimedia optimization and clean architecture.

## 📋 Descripción General

Este proyecto es una demostración técnica de un portfolio de alto rendimiento que integra:
- **Backend robusto** con Django Rest Framework
- **Frontend moderno** con Vue 3 
- **Optimización multimedia** avanzada
- **Arquitectura limpia** y escalable

## 🎯 Características Principales

### Backend (Django + DRF)
- API REST bien documentada
- Autenticación y autorización segura
- Optimización de consultas a base de datos
- Validación robusta de datos
- Sistema de caché inteligente

### Frontend (Vue 3)
- Componentes reutilizables y mantenibles
- Gestión de estado centralizada
- Optimización de carga de imágenes y multimedia
- Interfaz responsive y accesible
- Performance optimizado

### Multimedia
- Compresión inteligente de imágenes
- Lazy loading de contenido
- Formatos modernos (WebP, AVIF)
- CDN integration ready
- Carga progresiva de assets

## 🛠️ Stack Tecnológico

### Backend
- **Python 3.10+**
- **Django 4.x**
- **Django Rest Framework (DRF)**
- **PostgreSQL** (recomendado)
- **Redis** para caché

### Frontend
- **Vue 3**
- **Vite** (build tool)
- **Pinia** (state management)
- **Axios** para HTTP requests
- **TailwindCSS** para estilos

### DevOps & Tools
- **Docker** para containerización
- **Docker Compose** para orquestación local
- **GitHub Actions** para CI/CD
- **ESLint & Prettier** para code quality

## 📦 Estructura del Proyecto

```
.
├── backend/
│   ├── config/          # Configuración de Django
│   ├── apps/            # Aplicaciones Django
│   ├── requirements.txt  # Dependencias Python
│   └── manage.py
├── frontend/
│   ├── src/
│   │   ├── components/  # Componentes Vue
│   │   ├── views/       # Páginas/vistas
│   │   ├── stores/      # Estado con Pinia
│   │   └── App.vue
│   ├── package.json
│   └── vite.config.js
├── docker-compose.yml
└── README.md
```

## 🚀 Inicio Rápido

### Requisitos Previos
- Python 3.10+
- Node.js 16+
- Docker (opcional)
- PostgreSQL 13+ (opcional, puedes usar SQLite para desarrollo)

### Instalación Local

#### 1. Clonar el repositorio
```bash
git clone https://github.com/RubenVSM/max-benito-smeele-technical-samples.git
cd max-benito-smeele-technical-samples
```

#### 2. Configurar Backend
```bash
cd backend
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

#### 3. Configurar Frontend
```bash
cd frontend
npm install
npm run dev
```

La aplicación estará disponible en `http://localhost:5173`

### Con Docker
```bash
docker-compose up -d
```

## 📚 Documentación API

La documentación de la API está disponible en:
- **Swagger UI**: `http://localhost:8000/api/docs/swagger/`
- **ReDoc**: `http://localhost:8000/api/docs/redoc/`

## 🧪 Testing

### Backend
```bash
cd backend
python manage.py test
```

### Frontend
```bash
cd frontend
npm run test
npm run test:coverage
```

## 📊 Performance & Optimization

### Backend Optimizations
- Índices de base de datos optimizados
- Query optimization con select_related/prefetch_related
- Rate limiting y throttling
- Gzip compression
- Static files serving optimizado

### Frontend Optimizations
- Code splitting automático
- Tree shaking de dependencies
- Image optimization con formato moderno
- Service Worker para offline support
- Bundle size monitoring

## 🔒 Seguridad

- CSRF protection activado
- CORS configurado correctamente
- SQL injection prevención
- XSS protection
- Validación de entrada en cliente y servidor
- HTTPS en producción recomendado

## 🤝 Contribuir

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📝 Licencia

Este proyecto está disponible bajo licencia MIT. Ver archivo `LICENSE` para más detalles.

## 👤 Autor

**Rubén VSM**
- GitHub: [@RubenVSM](https://github.com/RubenVSM)
- Portfolio: Consulta otros proyectos en el perfil

## 📞 Contacto & Support

Para reportar issues o sugerencias, abre un issue en el repositorio.

---

**Última actualización**: Julio 2026
