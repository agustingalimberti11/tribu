# Tribu

## 📖 Descripción

**Tribu** es una plataforma web diseñada para conectar personas a través de actividades reales. La aplicación permite a los usuarios crear, explorar y participar en eventos cercanos como corridas, partidos de fútbol, mateadas, lecturas y muchas otras actividades sociales.

En Tribu creemos que las mejores experiencias se viven juntos. Unite a nuestra comunidad, participá en eventos reales y descubrí nuevas formas de disfrutar tu tiempo con otras personas.

## ✨ Características Principales

- **Registro y Autenticación**: Los usuarios pueden crear una cuenta, iniciar sesión y personalizar su perfil con intereses
- **Exploración de Eventos**: Navegá por eventos cercanos filtrados por categoría, fecha y ubicación
- **Creación de Eventos**: Creá tus propios eventos especificando título, descripción, fecha, hora, ubicación y capacidad
- **Participación en Eventos**: Unite a eventos que te interesen y conectá con otros participantes
- **Perfil de Usuario**: Gestioná tus eventos creados, visualizá tus participaciones y configurá tu cuenta
- **Detalles de Eventos**: Visualizá información completa de cada evento, participantes, comentarios y eventos similares

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura semántica de las páginas
- **CSS3**: Estilos personalizados y diseño responsive
- **Bootstrap 5.3.2**: Framework CSS para diseño responsive y componentes UI
- **JavaScript**: Interactividad y validación de formularios

## 📁 Estructura del Proyecto

```
tribu/
├── scss/                  # Código fuente SCSS
│   ├── abstracts/         # Variables, mixins, functions
│   ├── base/              # Reset, tipografía, animaciones
│   ├── components/        # Componentes reutilizables
│   ├── layout/            # Header, footer, container
│   ├── utilities/         # Utilidades y helpers
│   └── main.scss          # Archivo principal
├── css/
│   └── style.css          # CSS compilado desde SCSS
├── img/                   # Imágenes y recursos visuales
│   ├── logo.png
│   ├── img-principal-index.png
│   ├── explora-index.png
│   ├── participa-index.png
│   ├── registro-index.png
│   ├── futbol.jpg
│   ├── mates.jpg
│   ├── running.jpeg
│   ├── linkedin.jpg
│   └── instagram.png
├── pages/
│   ├── explora-eventos.html    # Página de exploración de eventos
│   ├── crear-evento.html       # Formulario para crear eventos
│   ├── detalle-evento.html     # Vista detallada de un evento
│   ├── perfil.html             # Perfil del usuario
│   └── registro.html           # Registro e inicio de sesión
├── index.html                  # Página principal
└── README.md                   # Este archivo
```

## 🚀 Funcionalidades

### Página Principal (`index.html`)
- Presentación de la plataforma
- Navegación a las secciones principales
- Tarjetas informativas sobre cómo usar la plataforma

### Explorar Eventos (`pages/explora-eventos.html`)
- Listado de eventos cercanos disponibles
- Botón para crear nuevos eventos
- Tarjetas con información resumida de cada evento
- Enlaces para unirse a eventos

### Crear Evento (`pages/crear-evento.html`)
- Formulario completo con validación
- Campos: título, descripción, fecha, hora, ubicación
- Selección de categoría (Deportes, Social, Cultural, Educativo, Otro)
- Capacidad máxima de participantes
- Subida de imagen del evento
- Requisitos opcionales (equipo, nivel, pago)

### Detalle de Evento (`pages/detalle-evento.html`)
- Información completa del evento
- Lista de participantes
- Sección de comentarios
- Eventos similares recomendados
- Botón para unirse al evento

### Perfil de Usuario (`pages/perfil.html`)
- Información del usuario (nombre, foto, calificación)
- Estadísticas (eventos creados, participaciones)
- Pestañas para:
  - **Mis Eventos**: Eventos creados por el usuario con opciones de editar/eliminar
  - **Participaciones**: Eventos en los que el usuario participa
  - **Configuración**: Edición de datos personales

### Registro/Inicio de Sesión (`pages/registro.html`)
- Formulario de inicio de sesión
- Formulario de registro con:
  - Datos personales (nombre, apellido, email)
  - Contraseña
  - Selección de intereses múltiples
  - Aceptación de términos y condiciones

## 🎨 Diseño

El proyecto utiliza un diseño moderno y responsive que se adapta a diferentes tamaños de pantalla:
- Diseño mobile-first
- Navegación responsive con menú hamburguesa en dispositivos móviles
- Paleta de colores con énfasis en verde para acciones principales
- Uso de Bootstrap para componentes consistentes y accesibles

## 📝 Uso

1. Abrí el archivo `index.html` en tu navegador web
2. Navegá por las diferentes secciones usando el menú de navegación
3. Registrate o iniciá sesión para acceder a todas las funcionalidades
4. Explorá eventos disponibles o creá uno nuevo
5. Unite a eventos que te interesen y conectá con otros usuarios

## 🔨 Compilación SCSS

Este proyecto utiliza SCSS para la organización de estilos. Para compilar:

```bash
# Instalar dependencias
npm install

# Compilar SCSS a CSS
npm run sass

# Modo watch (compila automáticamente)
npm run sass:watch
```

Ver `COMPILACION.md` para más detalles.

## 🔮 Próximas Mejoras

- Integración con backend para persistencia de datos
- Sistema de autenticación real
- Búsqueda y filtros avanzados de eventos
- Notificaciones de eventos
- Sistema de calificaciones y reseñas
- Chat entre participantes
- Integración con mapas para ubicaciones

## 👤 Autor

Desarrollado por [Agustín Galimberti](https://ar.linkedin.com/in/agustingalimberti)

---

**Tribu** - Conectá con personas a través de actividades reales
